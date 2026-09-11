# Where the figures in the bug-fix report came from

Five figures in [`bug_fixes.md`](./bug_fixes.md) were queried by a reviewer.
Each is answered below: the test figures with the output that produced them, the
other four with their source and calculation.

---

## 1. Test success, 70% (210 of 300) → 100% (303 of 303)

The **after** figure is correct. The **before** figure was mis-stated: the
correct figure is **117 of 177 (66.1%)**.

| | Commit | Date | Result |
| --- | --- | --- | --- |
| Before the fixes | [`66d2ab56`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/66d2ab56) | 2 July 2025 | 117 of 177 passing (66.1%), 32 suites |
| After the fixes | [`8360d8d6`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/8360d8d6) | 12 July 2025 | 303 of 303 passing (100%), 45 suites |

The full Jest output for both runs is committed:

- [`evidence/test-output-66d2ab56-before.txt`](./evidence/test-output-66d2ab56-before.txt)
- [`evidence/test-output-8360d8d6-after.txt`](./evidence/test-output-8360d8d6-after.txt)

`8360d8d6` is the commit the report was written against. To reproduce either:

```bash
git checkout 8360d8d6
pnpm install && pnpm db:deploy && npx jest --runInBand --verbose
```

Use **Node 19 or later**: the suite calls `crypto.randomUUID`, which Node
exposes as a global by default only from version 19.

Coverage for `8360d8d6` is committed as
[`evidence/coverage-clover-8360d8d6.xml`](./evidence/coverage-clover-8360d8d6.xml).

---

## 2. Database timeout errors, 25/day → fewer than 1/day

**Source.** Cloud Logging on the production project. The service logs through
Winston with `@google-cloud/logging-winston`.

**Calculation.** Log entries per day whose message matches Prisma's `P2024` and
the related connection-pool timeout errors.

---

## 3. Authentication failures, 12% → below 0.1%

**Source.** The Cloud Run request logs for the service, which record every
inbound request with its status code.

**Calculation.** Responses with status 401 or 403, divided by total requests in
the same window.

---

## 4. External API failures, 15% → 2%

**Source.** Cloud Logging — the DID/VC batch jobs. Each run logs its own size
and then the outcome of every call in that run, so the rate has both a numerator
and a denominator:

| File | Run size | Per call |
| --- | --- | --- |
| [`requestDIDVC/requestDID.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/8360d8d6/src/presentation/batch/requestDIDVC/requestDID.ts#L49-L81) | `🆕 Found N users without DID issuance request` | `✅ DID request created` / `❌ DID request failed` |
| [`requestDIDVC/requestVC.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/8360d8d6/src/presentation/batch/requestDIDVC/requestVC.ts#L64-L104) | `🆕 Found N PASSED evaluations without VC request` | `✅ VC requested` / `❌ VC request failed` |
| [`syncDIDVC/syncDID.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/8360d8d6/src/presentation/batch/syncDIDVC/syncDID.ts#L39-L140) | `📡 Found N processing DID issuance requests` | `✅ DID completed` / `❌ DID failed` |
| [`syncDIDVC/syncVC.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/8360d8d6/src/presentation/batch/syncDIDVC/syncVC.ts#L44-L170) | `📡 Found N processing VC issuance requests` | `✅ VC completed` / `External API call failed for VC job` |

The DID/VC HTTP client
([`libs/did.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/8360d8d6/src/infrastructure/libs/did.ts#L22-L43))
also logs every outbound call and every failure.

**Calculation.** Failed calls divided by the run size, over the same window.

---

## 5. Debugging time, improved by 60%

**Source.** The Prisma query and transaction logging added in upstream PR #346,
"Add logging and timeout mechanism for transactions"
([`52fc5221`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/52fc5221),
9 July 2025 — three days before the report).
[`src/infrastructure/prisma/client.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/8360d8d6/src/infrastructure/prisma/client.ts)
records a `duration` on every query and on every transaction, warns on queries
over 1000 ms and transactions over 3000 ms, and logs transaction timeouts at
warn level.

Before that change, a slow or timed-out transaction produced no duration and no
query detail, so diagnosing one meant reproducing it.

**Calculation.** None. The 60% is an assessment of that difference, not a
computed ratio. In the report it sits under *Development Efficiency*, beside
test reliability and code quality, as "Debug Time: Reduced by 60% due to
improved logging".

---

## On figures 2 to 4

The 2025 log data has passed the project's retention window (`_Default` bucket,
30 days), so those figures cannot be re-derived from the logs today. The sources
and calculations above are unchanged, and the current values for the same
queries are recorded under
[Runtime behaviour](./bug_fixes.md#runtime-behaviour) in the report.
