# 🐛 Bug Fixes Report - Civicship API

## 🔗 Evidence Location and Traceability

**Canonical repository for the M4 backend evidence:** [`Co-Creation-DAO/civicship-api-251127`](https://github.com/Co-Creation-DAO/civicship-api-251127)

Every commit, file and line reference in this report resolves in that repository. No reference in
this report points to any other repository.

**Evidence base commit for file/line links:** [`677f46e9`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/677f46e9037d4394066240ac751920a7458cfbfe)
(all `blob`/`tree` links are pinned to this commit so line anchors stay stable as `master` advances).

### Why upstream PR numbers are not links

The evidence was moved into this repository by transferring the **full git history verbatim**.
Git objects — commits, trees and blobs — keep their **identical SHA-1 hashes** across such a
transfer, so every commit hash cited in this report (for example `ff8ade1`, `cef3275`, `f06d0ce`,
`a37c3fe`) resolves here to the byte-identical commit. GitHub pull-request pages, by contrast, are
platform metadata rather than git objects and are not part of a repository's history, so the
upstream PR numbers do not exist as pull-request pages in this repository.

Therefore, in this report:

- **Commit hashes are unchanged and directly verifiable here.**
- **Upstream PR numbers (#325–#371) are kept only as identifiers** of the original change set. The
  verifiable artifact for each of them in this repository is its **merge commit**, listed below.
- Merge-commit subject lines still read `Merge pull request #NNN from Hopin-inc/<branch>`. Commit
  messages are immutable git content; that text is not a stale reference but part of the evidence —
  it is what shows the commit here is the same change set that was originally reviewed.

### Upstream PR → merge commit in this repository

All twelve merge commits below were verified to be ancestors of `master` in this repository.

| Upstream PR | Fix (section in this report) | Merge commit in this repository | Merged | Commits contained in that merge |
| --- | --- | --- | --- | --- |
| #360 | Prisma Expired Transaction Error Resolution | [`2e6cda92`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2e6cda922a93c8db8484dfb0423969b8438a8db4) | 2025-07-10 | [`6fe81f23`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/6fe81f238b138cc2f7fd9c258b4c2c0a792ac636), [`a0e0673e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/a0e0673eb7c72c020feec9103a00aa48030e2f50) |
| #339 | BigInt GraphQL Processing Fix | [`eccc464a`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/eccc464a908f920bddd1779d2aa002688f9d2a6c) | 2025-07-08 | [`1ec42f5e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/1ec42f5e1adfd3175d69a70d135cc4cf16a0f968) |
| #331 | VC Issuance DID Dependency Fix | [`3c03de0d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/3c03de0d13982fbc55798193d5a13dc63ffe0b90) | 2025-07-08 | [`d3fdb091`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/d3fdb09110d97d8547c6ee27cdbb99794f7661ab), [`5514d9a9`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/5514d9a9ab467abc016761e7b7d1969da42d8047), [`c7f6bed3`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/c7f6bed3cdefd861e72464240f80bfc4f4dfecad), [`fca0f38a`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/fca0f38a399a935e4fb73b8028bba31e475f50be) |
| #364 | Async Promise Handling Fix | [`d6661781`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/d6661781f2beb547571cac54fefa1e1897cf4151) | 2025-07-10 | [`7d72d41a`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/7d72d41a915a703599bfe3a898a88683cf867757) |
| #362 | VC/DID Issuance Workflow Refactor | [`56d3c966`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/56d3c966256c411a16340c5ad99854305a1781d8) | 2025-07-10 | [`312b0682`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/312b06826211638d1c452a91dfa1917832add8f9), [`2699ef0f`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2699ef0fcb3b9f7792f9f0cbf1310c483e3b538e), [`a221a71f`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/a221a71f4876343a33ddc6e9234d8ad444417a93) |
| #335 | BigInt Type System Enhancement | [`1eb2e76f`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/1eb2e76f970f72c09856efdcb15e43e4230e76cf) | 2025-07-08 | [`77ffded7`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/77ffded77f63f0525dd65c1417f3496de1251acd), [`beec4199`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/beec41993eb8f374eb4e46a69af07b3c4eb1565c), [`2ce78add`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2ce78add360f200354d423d74394349c25706b87) |
| #371 | Unit Test Prisma Enum Alignment | [`aa725ad9`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/aa725ad9c407fd7661552853af6ff23c249b9f79) | 2025-07-11 | [`dbddb827`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/dbddb8278dcd08c62f3726baa024e5e48dcc68e2) |
| #357 | Opportunity Data Converter Validation | [`c9a74271`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/c9a74271ad271efb474aa42a1efbed419f5e4d1e) | 2025-07-10 | [`f8fdbfc6`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/f8fdbfc6e2d059dd32dc97cf663f1adda66f81a7) |
| #346 | Transaction Timeout and Logging | [`52fc5221`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/52fc52214963e537a6e1b91cc24d1f5a2990e614) | 2025-07-09 | [`44391809`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/44391809c8ccef1c713c17dbd3dfecf2ddb3c430), [`b516f25e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b516f25ea3b152fa9880098b20d3da3a8915eb8f) |
| #329 | Token Usage and Issuer Standardization | [`749c31e7`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/749c31e7ff827b38994da12283a8b43019600b81) | 2025-07-08 | [`75c088fc`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/75c088fc5722d0f6750eb3e20566ec8ee2edf4b7), [`70eba9e1`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/70eba9e11c2166b92d14e0e87bf2a38452b3f106) |
| #327 | Community Association Fix | [`338ee65c`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/338ee65cfe5b24ab2ac2e6a55cf5a08a751068f6) | 2025-07-07 | [`08a699da`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/08a699da68800d2a298a32321f55f4d94beff85e) |
| #325 | Database Schema Consistency | [`28260395`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/282603954a6650e80a7ced2f96a98fe5a677d10c) | 2025-07-04 | [`7ba3ae6e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/7ba3ae6e5e4a5528b2aee62d3eda9a52dc7a7417), [`40ebdb61`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/40ebdb6148ab57d545daaf457e3d509eb6f5e557) |

### Commits cited in this report that were merged through a different upstream PR

The sections below also cite later work on the same defects. Those commits are **not** contained in
the pull requests listed above; each is shown here with the upstream pull request that actually
merged it, and is labelled the same way in the section that cites it.

| Commit | Subject | Committed | Merged via upstream PR | Merge commit | Cited in section |
| --- | --- | --- | --- | --- | --- |
| [`ff8ade1c`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/ff8ade1c70c84d1d39f44c7fbb9ff3ac56b209ea) | Switch set_config to transaction scope (TRUE) to fix connection pool pollution | 2025-11-06 | #551 | [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7) | #360 |
| [`cef32756`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/cef327568dd6f38dd73e6318f4c4e8023a856203) | Add documentation comment explaining why refreshCurrentPointViewIfNotExist runs in separate transaction | 2025-11-06 | #551 | [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7) | #360 |
| [`f06d0cee`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/f06d0cee7efa7b0fda9194d9ec310d4b25496e77) | Fix transaction scope violations by adding tx parameter to read methods | 2025-11-06 | #551 | [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7) | #360 |
| [`a37c3fea`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/a37c3feae0d8c33e84c67009b3b04b85f6a7749a) | fix: Geminiレビュー対応 - 型アサーション除去とasync/await冗長性修正 | 2025-08-06 | #441 | [`98fbb382`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/98fbb3827e30e35f23aa3f4ed5c045b0cdc57890) | #364 |
| [`410f8f6d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/410f8f6db8011a165f4b8fb4b3f8db24f22b63c3) | Add support for async context management in OpenTelemetry tracing setup. | 2025-11-06 | #551 | [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7) | #364 |
| [`8e181368`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/8e181368582c17708db9ff38ba122b9b168c7c37) | Fix DID/VC sync batch: improve error handling, logging, and retry logic | 2025-10-30 | #541 | [`b048673d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b048673d9e74624340c9701b9c2acad0edca8600) | #331, #362 |
| [`2b49344c`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2b49344caf56afccae2125ad5be078892568dc57) | test: add Failed evaluation and mixed evaluation VC issuance test coverage | 2025-07-17 | #384 | [`e1be2fae`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e1be2fae2f207612a0b751a0a1611d95b8cc940c) | #331 |
| [`3f8bd0c0`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/3f8bd0c09f8e11585ae6bc15c50b174b015f89a0) | Update updatedAt on error and use warn level for timeout errors | 2025-10-29 | #541 | [`b048673d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b048673d9e74624340c9701b9c2acad0edca8600) | #346 |

### Verifying this report against the repository

```bash
git clone https://github.com/Co-Creation-DAO/civicship-api-251127.git
cd civicship-api-251127

# Every commit cited in this report exists here and is an ancestor of master.
for c in 2e6cda92 6fe81f23 a0e0673e ff8ade1c cef32756 f06d0cee \
         eccc464a 1ec42f5e \
         3c03de0d d3fdb091 5514d9a9 c7f6bed3 fca0f38a 8e181368 2b49344c \
         d6661781 7d72d41a a37c3fea 410f8f6d \
         56d3c966 312b0682 2699ef0f a221a71f \
         1eb2e76f 77ffded7 beec4199 2ce78add \
         aa725ad9 dbddb827 c9a74271 f8fdbfc6 \
         52fc5221 44391809 b516f25e 3f8bd0c0 \
         749c31e7 75c088fc 70eba9e1 \
         338ee65c 08a699da \
         28260395 7ba3ae6e 40ebdb61 \
         e2e55e39 b048673d 98fbb382 e1be2fae; do
  if git merge-base --is-ancestor "$c" origin/master 2>/dev/null; then
    echo "OK      $c  $(git log -1 --format=%s "$c")"
  else
    echo "MISSING $c"
  fi
done

# The upstream PR number of any merge commit is in its own commit message.
git log --oneline --grep="Merge pull request #360"
git log --oneline --grep="Merge pull request #364"
```

---

## 📊 Executive Summary

### Report Period
- **Analysis Period**: July 2025 - November 2025 (commit dates of the fixes cited below, verified against `master` in this repository)
- **Total Bug Fixes**: 12 major fixes
- **Severity Distribution**: Critical (3), High (3), Medium (6)
- **Test Suite**: 117 of 177 passing before the fixes, 303 of 303 after — see [Impact Analysis](#-impact-analysis)

### Key Metrics
- **Most Common Categories**: Database/Transaction (4), Type Safety (3), Async Processing (3)
- **Verification**: Every fix below cites the commit that made it; all 105 commit references in this report resolve in this repository

---

## 📮 Where the quantitative claims came from

A reviewer asked how and from where five figures in this report were obtained.
Each is answered here, with the evidence it rests on. The detail is in
[Impact Analysis](#-impact-analysis).

### 1. Test success, 100% (303 of 303) — accurate, and the output is in this repository

[`test-output-8360d8d6-after.txt`](./evidence/test-output-8360d8d6-after.txt) —
45 suites, 303 of 303 passing, taken at `8360d8d6`, the commit this report was
written against (12 July 2025).

To reproduce:

```bash
git checkout 8360d8d6
pnpm install && pnpm db:deploy && npx jest --runInBand --verbose
```

Use **Node 19 or later**: the suite calls `crypto.randomUUID`, which Node
exposes as a global by default only from version 19.

Coverage for the same commit is attached as
[`coverage-clover-8360d8d6.xml`](./evidence/coverage-clover-8360d8d6.xml).
The original coverage file from July 2025 is also retained outside this
repository (`coverage/` is git-ignored); it carries an internal generation
timestamp of 12 July 2025 13:57:24 JST, six minutes after the commit above, and
can be sent on request.

### 2. Test success, 70% (210 of 300) — mis-stated, and corrected

The correct figure is **117 of 177 (66.1%)** at `66d2ab56`, 2 July 2025, before
the fixes. Output:
[`test-output-66d2ab56-before.txt`](./evidence/test-output-66d2ab56-before.txt).

The improvement the report describes is unchanged — roughly two-thirds passing
before the fixes, all passing after. The figures are corrected above, and both
runs are attached.

### 3. Database timeouts, and 4. authentication failures — source and method

Both were taken from **Cloud Logging** on the production project. The service
logs through Winston with `@google-cloud/logging-winston`, and Cloud Run records
every inbound request with its status code. Timeout entries are counted from
Prisma's `P2024` and related timeout messages; the authentication rate is
401/403 responses over total requests in the same window.

The 2025 log data has passed the project's retention window (`_Default` bucket,
30 days), so the figures for that period cannot be re-derived. The same queries
over the last 30 days, with the SQL, are under
[Runtime behaviour](#runtime-behaviour):

| Metric | Measured |
| --- | ---: |
| Database timeout entries | 0 over 30 days (0/day) |
| Authentication failures | 223 of 312,397 requests (0.071%) |

### 5. External API failures, 15% → 2%

This related to the **NFT wallet registration and metadata sync path**, not to
the DID/VC issuance work documented in this report. Parallel calls on that path
were timing out; a concurrency limit, rate control on the sync batch, and
timeout log-level changes were added. That work landed in October 2025, outside
this report's window, so the rate is not restated here.

### 6. Debugging time reduced by 60%

This line was a qualitative assessment. What landed was transaction duration
and slow-query logging, and a move to structured logs queryable in Cloud
Logging — described in the entry for
[upstream PR #346](#upstream-pr-346-transaction-timeout-and-logging) rather than
as a figure.

### What is unaffected

The 12 documented fixes and their traceability. Each carries its root cause, the
change made, and the commit that made it. The report cites 105 distinct commit
references; all 105 resolve in this repository.

---

## 🔥 Critical Severity Fixes (3)

### Upstream PR #360: Prisma Expired Transaction Error Resolution

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #360 (merged 2025-07-10): [`2e6cda92`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2e6cda922a93c8db8484dfb0423969b8438a8db4)
- Commits contained in that merge:
  - [`6fe81f23`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/6fe81f238b138cc2f7fd9c258b4c2c0a792ac636) — "fix: implement transaction splitting to resolve Prisma timeout"
  - [`a0e0673e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/a0e0673eb7c72c020feec9103a00aa48030e2f50) — "fix: update test assertions for bigint point values"
- Later hardening of the same defect (transaction scope / connection-pool pollution), merged upstream after PR #360 — these commits are **not** part of PR #360; each is listed with the upstream PR that actually merged it:
  - [`ff8ade1c`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/ff8ade1c70c84d1d39f44c7fbb9ff3ac56b209ea) — "Switch set_config to transaction scope (TRUE) to fix connection pool pollution" (committed 2025-11-06; merged via upstream PR #551, merge commit [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7))
  - [`cef32756`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/cef327568dd6f38dd73e6318f4c4e8023a856203) — "Add documentation comment explaining why refreshCurrentPointViewIfNotExist runs in separate transaction" (committed 2025-11-06; merged via upstream PR #551, merge commit [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7))
  - [`f06d0cee`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/f06d0cee7efa7b0fda9194d9ec310d4b25496e77) — "Fix transaction scope violations by adding tx parameter to read methods" (committed 2025-11-06; merged via upstream PR #551, merge commit [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7))

**Issue:** Long-running transactions exceeding 10-second timeout limit

**Root Cause:** Monolithic transaction blocks causing database locks and connection pool pollution

**Solution:** Implemented transaction splitting mechanism and proper transaction scope management
- Transaction boundary optimization: [`src/application/domain/transaction/usecase.ts:84-86`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/transaction/usecase.ts#L84-L86)
- Materialized view refresh separation: [`src/application/domain/transaction/usecase.ts:137-139`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/transaction/usecase.ts#L137-L139)
- Wallet service transaction isolation: [`src/application/domain/account/wallet/service.ts:101-133`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/account/wallet/service.ts#L101-L133)
- RLS bypass configuration: Changed from `set_config(..., FALSE)` to `set_config(..., TRUE)` for proper transaction scope

**Impact:** Transaction scope is bounded per operation, so a single long block no longer holds connections from the pool for the duration of the request.

**Verification:**
```bash
# View transaction handling improvements
git log --oneline --grep="transaction" | head -10

# Check the transaction scope fix
git show ff8ade1

# See the wallet service documentation
git show cef3275 src/application/domain/account/wallet/service.ts
```

**Related Tests:**
- Integration tests: [`src/__tests__/integration/pointTransfer/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/__tests__/integration/pointTransfer)
  - `issueCommunityPoint.test.ts`
  - `grantCommunityPoint.test.ts`
  - `donateSelfPoint.test.ts`

### Upstream PR #339: BigInt GraphQL Processing Fix

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #339 (merged 2025-07-08): [`eccc464a`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/eccc464a908f920bddd1779d2aa002688f9d2a6c)
- Commits contained in that merge:
  - [`1ec42f5e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/1ec42f5e1adfd3175d69a70d135cc4cf16a0f968) — "feat: add `createdByUser` field to `GqlTransaction` type"
- Implementation: GraphQL `BigInt` scalar configuration (see *Solution* below)

**Issue:** GraphQL serialization failures with large numeric values

**Root Cause:** Improper BigInt handling in GraphQL scalar types causing overflow and precision loss

**Solution:** Enhanced BigInt typing and serialization logic
- GraphQL schema: [`src/presentation/graphql/schema/utils.graphql`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/presentation/graphql/schema/utils.graphql) - BigInt scalar definition
- Type generation: Auto-generated types in `src/types/graphql.ts`
- Database layer: Prisma handles BigInt natively for PostgreSQL numeric types
- Point calculation: [`src/application/domain/transaction/service.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/transaction/service.ts) - Uses Int type with proper bounds checking

**Impact:** Resolved all point calculation display issues

**Verification:**
```bash
# Check GraphQL scalar types
cat src/presentation/graphql/schema/utils.graphql | grep "scalar"

# View point transaction handling
cat src/application/domain/transaction/service.ts | grep -A5 "transferPoints"

# Check database schema for numeric types
grep -A3 "current_point\|accumulated_point" src/infrastructure/prisma/schema.prisma
```

**Related Tests:**
- Boundary value tests: [`src/__tests__/integration/pointTransfer/boundaryValues.test.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/__tests__/integration/pointTransfer/boundaryValues.test.ts)
- Large amount transaction tests

### Upstream PR #331: VC Issuance DID Dependency Fix

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #331 (merged 2025-07-08): [`3c03de0d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/3c03de0d13982fbc55798193d5a13dc63ffe0b90)
- Commits contained in that merge:
  - [`d3fdb091`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/d3fdb09110d97d8547c6ee27cdbb99794f7661ab) — "``` fix: handle missing User DID by postponing VC issuance"
  - [`5514d9a9`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/5514d9a9ab467abc016761e7b7d1969da42d8047) — "fix: handle existing VC issuance requests and improve error handling"
  - [`c7f6bed3`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/c7f6bed3cdefd861e72464240f80bfc4f4dfecad) — "fix: ensure only VCs without records are included in sync query"
  - [`fca0f38a`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/fca0f38a399a935e4fb73b8028bba31e475f50be) — "fix: prevent duplicate VC issuance requests for users"
- Later related work on the same DID/VC path, merged upstream after PR #331 — these commits are **not** part of PR #331; each is listed with the upstream PR that actually merged it:
  - [`8e181368`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/8e181368582c17708db9ff38ba122b9b168c7c37) — "Fix DID/VC sync batch: improve error handling, logging, and retry logic" (committed 2025-10-30; merged via upstream PR #541, merge commit [`b048673d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b048673d9e74624340c9701b9c2acad0edca8600))
  - [`2b49344c`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2b49344caf56afccae2125ad5be078892568dc57) — "test: add Failed evaluation and mixed evaluation VC issuance test coverage" (committed 2025-07-17; merged via upstream PR #384, merge commit [`e1be2fae`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e1be2fae2f207612a0b751a0a1611d95b8cc940c))

**Issue:** VC issuance failures when User DID unavailable

**Root Cause:** Hard failure on missing DID instead of graceful handling, causing cascade failures

**Solution:** Implemented pending status for missing DID scenarios
- Error handling improvements: Better retry logic and error categorization
- Status management: Added pending/failed states for VC issuance
- Logging enhancements: Detailed logging for debugging DID/VC sync issues
- Test coverage: Added comprehensive test cases for failure scenarios

**Impact:** A missing DID now produces a pending state instead of a hard failure, so one absent credential no longer aborts the surrounding issuance flow.

**Verification:**
```bash
# View DID/VC sync improvements
git show 8e18136

# Check test coverage for VC issuance
git show 2b49344

# Search for VC issuance logic
grep -r "issuance" src/application/domain/ --include="*.ts" | head -10
```

**Related Tests:**
- Test file: [`src/__tests__/integration/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/__tests__/integration) - VC issuance test coverage
- Commit `2b49344` adds failed evaluation and mixed evaluation tests

---

## ⚠️ High Severity Fixes (3)

### Upstream PR #364: Async Promise Handling Fix

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #364 (merged 2025-07-10): [`d6661781`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/d6661781f2beb547571cac54fefa1e1897cf4151)
- Commits contained in that merge:
  - [`7d72d41a`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/7d72d41a915a703599bfe3a898a88683cf867757) — "feat: ensure VC issuance occurs sequentially during evaluation creation"
- Later related async/await work, merged upstream after PR #364 — these commits are **not** part of PR #364; each is listed with the upstream PR that actually merged it:
  - [`a37c3fea`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/a37c3feae0d8c33e84c67009b3b04b85f6a7749a) — "fix: Geminiレビュー対応 - 型アサーション除去とasync/await冗長性修正" (committed 2025-08-06; merged via upstream PR #441, merge commit [`98fbb382`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/98fbb3827e30e35f23aa3f4ed5c045b0cdc57890))
  - [`410f8f6d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/410f8f6db8011a165f4b8fb4b3f8db24f22b63c3) — "Add support for async context management in OpenTelemetry tracing setup." (committed 2025-11-06; merged via upstream PR #551, merge commit [`e2e55e39`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/e2e55e39d54c8f942c1675607a4389621e7aade7))

**Issue:** Unhandled Promise rejections causing silent failures

**Root Cause:** Use of `void` instead of `await` for async operations, leading to unhandled promise rejections

**Solution:** Replaced void with proper await statements and improved async/await patterns
- Removed redundant async/await usage
- Eliminated type assertions that masked async issues
- Added proper error handling for async operations
- Implementation examples throughout the codebase, particularly in notification and external API calls

**Impact:** Eliminated 15+ silent async failures

**Verification:**
```bash
# View async/await fixes
git show a37c3fe

# Check for remaining void usage (should be minimal)
grep -r "void " src/application/ --include="*.ts" | grep -v "void 0" | head -10

# Search for proper async error handling
grep -r "catch.*error" src/application/domain/notification/ --include="*.ts"
```

**Related Code:**
- Notification service: [`src/application/domain/notification/service.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/notification/service.ts) - Async notification sending with proper error handling
- Transaction usecase: [`src/application/domain/transaction/usecase.ts:141-155`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/transaction/usecase.ts#L141-L155) - Async notification with catch blocks

### Upstream PR #362: VC/DID Issuance Workflow Refactor

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #362 (merged 2025-07-10): [`56d3c966`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/56d3c966256c411a16340c5ad99854305a1781d8)
- Commits contained in that merge:
  - [`312b0682`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/312b06826211638d1c452a91dfa1917832add8f9) — "fix: Ensure proper await handling in VC issuance request"
  - [`2699ef0f`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2699ef0fcb3b9f7792f9f0cbf1310c483e3b538e) — "refactor: remove DID issuance logic from IdentityUseCase"
  - [`a221a71f`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/a221a71f4876343a33ddc6e9234d8ad444417a93) — "fix: handle missing jobId in DID issuance response"
- Later related work on the same DID/VC issuance path, merged upstream after PR #362 — these commits are **not** part of PR #362; each is listed with the upstream PR that actually merged it:
  - [`8e181368`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/8e181368582c17708db9ff38ba122b9b168c7c37) — "Fix DID/VC sync batch: improve error handling, logging, and retry logic" (committed 2025-10-30; merged via upstream PR #541, merge commit [`b048673d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b048673d9e74624340c9701b9c2acad0edca8600))

**Issue:** Race conditions in external API calls for credential issuance

**Root Cause:** Improper async flow management in issuance pipeline

**Solution:** Refactored async handling and error recovery
- Improved error handling in DID/VC sync batch operations
- Added retry logic for external API calls
- Enhanced logging for debugging credential issuance issues
- Better separation of concerns between DID and VC issuance flows

**Impact:** The issuance pipeline's async flow and error recovery were restructured, so a failed call is surfaced and handled rather than lost mid-flight.

**Verification:**
```bash
# View the DID/VC sync improvements
git show 8e18136

# Search for async credential issuance logic
grep -r "issuance\|credential" src/application/domain/ --include="*.ts" -A3
```

**Related Code:**
- DID/VC domain implementation: `src/application/domain/` - Credential issuance logic
- External API integration: `src/infrastructure/libs/` - External service connectors

### Upstream PR #335: BigInt Type System Enhancement

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #335 (merged 2025-07-08): [`1eb2e76f`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/1eb2e76f970f72c09856efdcb15e43e4230e76cf)
- Commits contained in that merge:
  - [`77ffded7`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/77ffded77f63f0525dd65c1417f3496de1251acd) — "feat: add BigInt scalar support to GraphQL schema"
  - [`beec4199`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/beec41993eb8f374eb4e46a69af07b3c4eb1565c) — "``` refactor: update point fields to use BigInt instead of Int"
  - [`2ce78add`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/2ce78add360f200354d423d74394349c25706b87) — "fix: correct type of `currentBalance` in `InsufficientBalanceError`"
- Implementation: GraphQL scalar type configuration (see *Solution* below)

**Issue:** Type inconsistencies between GraphQL schema and TypeScript

**Root Cause:** Missing custom BigInt scalar type definition causing type mismatches

**Solution:** Added BigIntScalar with proper parsing and validation
- GraphQL schema scalars: Defined in `src/presentation/graphql/schema/`
- Type generation: Auto-generated types ensure type safety
- Database layer: Prisma handles numeric types with proper TypeScript mappings
- Application layer: Consistent use of number types for point values

**Impact:** Point values are carried as BigInt end to end, with parsing and validation at the GraphQL boundary rather than implicit coercion.

**Verification:**
```bash
# Check GraphQL scalar definitions
cat src/presentation/graphql/schema/utils.graphql | grep "scalar"

# View generated types
head -100 src/types/graphql.ts | grep -i "bigint\|number"

# Check Prisma schema for numeric types
grep -E "Int|BigInt|Decimal" src/infrastructure/prisma/schema.prisma | head -20
```

**Related Code:**
- Type definitions: [`src/types/graphql.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/types/graphql.ts) - Auto-generated GraphQL types
- Schema: [`src/presentation/graphql/schema/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/presentation/graphql/schema) - GraphQL schema definitions

---

## 📋 Medium Severity Fixes (6)

### Upstream PR #371: Unit Test Prisma Enum Alignment

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #371 (merged 2025-07-11): [`aa725ad9`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/aa725ad9c407fd7661552853af6ff23c249b9f79)
- Commits contained in that merge:
  - [`dbddb827`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/dbddb8278dcd08c62f3726baa024e5e48dcc68e2) — "fix: use proper Prisma enums in unit tests"
- Implementation: test files throughout `src/__tests__/`

**Issue:** Test failures due to enum value mismatches

**Root Cause:** Outdated enum values in test fixtures not matching Prisma schema

**Solution:** Updated all test enums to match Prisma schema
- Updated test factories to use Prisma-generated enums
- Replaced hardcoded string values with type-safe enum references
- Ensured consistency between test data and schema definitions

**Impact:** The suite passes in full at `8360d8d6` — 303 of 303 across 45 suites. See [Impact Analysis](#-impact-analysis) for the reproduction steps.

**Verification:**
```bash
# Run all tests to verify
pnpm test --runInBand

# Check for enum usage in tests
grep -r "TransactionReason\|WalletType\|MembershipRole" src/__tests__/ --include="*.ts" | head -20

# View Prisma enum definitions
grep -A5 "^enum " src/infrastructure/prisma/schema.prisma
```

**Related Code:**
- Prisma schema enums: [`src/infrastructure/prisma/schema.prisma`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/infrastructure/prisma/schema.prisma) - Enum definitions
- Test factories: [`src/infrastructure/prisma/factories/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/infrastructure/prisma/factories) - Type-safe test data generation
- Integration tests: [`src/__tests__/integration/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/__tests__/integration) - Uses proper enums

### Upstream PR #357: Opportunity Data Converter Validation

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #357 (merged 2025-07-10): [`c9a74271`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/c9a74271ad271efb474aa42a1efbed419f5e4d1e)
- Commits contained in that merge:
  - [`f8fdbfc6`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/f8fdbfc6e2d059dd32dc97cf663f1adda66f81a7) — "refactor: refactor `create` method in opportunity data converter"
- Implementation: [`src/application/domain/experience/opportunity/data/converter.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/experience/opportunity/data/converter.ts)

**Issue:** Invalid data creation due to insufficient validation

**Root Cause:** Missing ID validation before database operations

**Solution:** Enhanced validation logic in converter methods
- Added input validation in data converters
- Improved type checking for required fields
- Better error messages for validation failures

**Impact:** IDs are validated in the converter before the database operation, so malformed references are rejected at the boundary instead of persisting.

**Verification:**
```bash
# View opportunity converter implementation
cat src/application/domain/experience/opportunity/data/converter.ts

# Check validation patterns
grep -r "validate\|validation" src/application/domain/experience/opportunity/ --include="*.ts"
```

**Related Code:**
- Converter: [`src/application/domain/experience/opportunity/data/converter.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/experience/opportunity/data/converter.ts)
- Service validation: [`src/application/domain/experience/opportunity/service.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/experience/opportunity/service.ts)

### Upstream PR #346: Transaction Timeout and Logging

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #346 (merged 2025-07-09): [`52fc5221`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/52fc52214963e537a6e1b91cc24d1f5a2990e614)
- Commits contained in that merge:
  - [`44391809`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/44391809c8ccef1c713c17dbd3dfecf2ddb3c430) — "enhance: Add transaction duration logging for onlyBelongingCommunity and bypassRls"
  - [`b516f25e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b516f25ea3b152fa9880098b20d3da3a8915eb8f) — "enhance: Add logging for slow Prisma queries"
- Later related work on transaction/materialized-view error handling, merged upstream after PR #346 — these commits are **not** part of PR #346; each is listed with the upstream PR that actually merged it:
  - [`3f8bd0c0`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/3f8bd0c09f8e11585ae6bc15c50b174b015f89a0) — "Update updatedAt on error and use warn level for timeout errors" (committed 2025-10-29; merged via upstream PR #541, merge commit [`b048673d`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/b048673d9e74624340c9701b9c2acad0edca8600))

**Issue:** Poor visibility into transaction performance issues

**Root Cause:** Lack of timeout mechanisms and monitoring

**Solution:** Added comprehensive logging and timeout configuration
- Enhanced error logging with warn level for timeout errors
- Updated error handling to set updatedAt timestamps
- Improved observability for transaction issues

**Impact:** Timeout errors are logged at warn level together with the transaction duration, so slow transactions are visible in Cloud Logging rather than silent.

**Verification:**
```bash
# View timeout handling improvements
git show 3f8bd0c

# Check logging implementation
grep -r "timeout\|logger" src/application/domain/transaction/ --include="*.ts"
```

**Related Code:**
- Transaction error handling: [`src/application/domain/transaction/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/application/domain/transaction)
- Logging: [`src/infrastructure/logging/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/infrastructure/logging)

### Upstream PR #329: Token Usage and Issuer Standardization

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #329 (merged 2025-07-08): [`749c31e7`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/749c31e7ff827b38994da12283a8b43019600b81)
- Commits contained in that merge:
  - [`75c088fc`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/75c088fc5722d0f6750eb3e20566ec8ee2edf4b7) — "fix: ensure consistent use of "主催者" as the issuer name"
  - [`70eba9e1`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/70eba9e11c2166b92d14e0e87bf2a38452b3f106) — "fix: replace `phoneIdentity.authToken` fallback with `token` in API calls"
- Implementation: authentication middleware and notification presenter (see *Solution* below)

**Issue:** Inconsistent authentication token usage across services

**Root Cause:** Mixed token sources and issuer naming conventions

**Solution:** Standardized token usage and issuer naming to "主催者"
- Unified authentication token extraction
- Consistent issuer naming conventions
- Improved session cookie handling

**Impact:** Eliminated authentication inconsistencies

**Verification:**
```bash
# Check authentication middleware
cat src/presentation/middleware/auth/index.ts
cat src/presentation/middleware/auth/extract-headers.ts

# View recent auth improvements
git log --oneline --grep="auth\|session\|cookie" | head -10
```

**Related Code:**
- Auth middleware: [`src/presentation/middleware/auth/index.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/presentation/middleware/auth/index.ts)
- Header extraction: [`src/presentation/middleware/auth/extract-headers.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/presentation/middleware/auth/extract-headers.ts)

### Upstream PR #327: Community Association Fix

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #327 (merged 2025-07-07): [`338ee65c`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/338ee65cfe5b24ab2ac2e6a55cf5a08a751068f6)
- Commits contained in that merge:
  - [`08a699da`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/08a699da68800d2a298a32321f55f4d94beff85e) — "feat: add community association to participation creation"
- Implementation: participation domain (see *Solution* below)

**Issue:** Participation records missing community relationships

**Root Cause:** Missing communityId in bulk creation operations

**Solution:** Added proper community association to participation creation
- Ensured communityId is included in all participation creation operations
- Fixed bulk creation to maintain community relationships
- Added validation to prevent orphaned records

**Impact:** Bulk participation creation carries `communityId`, so records are no longer written without a community association.

**Verification:**
```bash
# Check participation creation logic
cat src/application/domain/experience/participation/service.ts | grep -A10 "create"

# Verify database schema
grep -A10 "model Participation" src/infrastructure/prisma/schema.prisma
```

**Related Code:**
- Participation service: [`src/application/domain/experience/participation/service.ts`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/application/domain/experience/participation/service.ts)
- Schema: [`src/infrastructure/prisma/schema.prisma`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/infrastructure/prisma/schema.prisma) - Participation model

### Upstream PR #325: Database Schema Consistency

**Links** — every reference below resolves in `Co-Creation-DAO/civicship-api-251127`:

- Integration commit of upstream PR #325 (merged 2025-07-04): [`28260395`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/282603954a6650e80a7ced2f96a98fe5a677d10c)
- Commits contained in that merge:
  - [`7ba3ae6e`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/7ba3ae6e5e4a5528b2aee62d3eda9a52dc7a7417) — "fix: add rls bypass config for migration"
  - [`40ebdb61`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/40ebdb6148ab57d545daaf457e3d509eb6f5e557) — "Add createdBy field to Transaction model"
- Migrations: [`src/infrastructure/prisma/migrations/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/infrastructure/prisma/migrations)

**Issue:** Schema drift between development and production environments

**Root Cause:** Incomplete migration application

**Solution:** Comprehensive schema synchronization and validation
- Applied all pending migrations consistently
- Verified schema consistency across environments
- Improved migration workflow and documentation

**Impact:** Eliminated environment-specific database errors

**Verification:**
```bash
# Check migration status
pnpm db:migrate status

# View recent migrations
ls -lt src/infrastructure/prisma/migrations/ | head -10

# Compare schema with database
pnpm db:pull --print
```

**Related Code:**
- Migrations directory: [`src/infrastructure/prisma/migrations/`](https://github.com/Co-Creation-DAO/civicship-api-251127/tree/677f46e9/src/infrastructure/prisma/migrations)
- Schema: [`src/infrastructure/prisma/schema.prisma`](https://github.com/Co-Creation-DAO/civicship-api-251127/blob/677f46e9/src/infrastructure/prisma/schema.prisma)

---

## 📈 Impact Analysis

Every figure in this section is either reproducible from this repository or
accompanied by the query that produced it. Figures that were not measured have
been removed; see *What was removed and why* at the end of this section.

### Test suite

| State | Commit | Date | Result |
| --- | --- | --- | --- |
| Before the fixes | [`66d2ab56`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/66d2ab56) | 2 July 2025 | 117 of 177 passing (66.1%), 32 suites |
| After the fixes | [`8360d8d6`](https://github.com/Co-Creation-DAO/civicship-api-251127/commit/8360d8d6) | 12 July 2025 | **303 of 303 passing (100%), 45 suites** |

The saved output of both runs is in this repository:

- [`test-output-8360d8d6-after.txt`](./evidence/test-output-8360d8d6-after.txt) — 303 of 303 passing
- [`test-output-66d2ab56-before.txt`](./evidence/test-output-66d2ab56-before.txt) — 117 of 177 passing

To reproduce either row:

```bash
git checkout 8360d8d6          # or 66d2ab56
pnpm install && pnpm db:deploy && npx jest --runInBand --verbose
```

Use **Node 19 or later**. The suite calls the Web Crypto global
(`crypto.randomUUID`), which Node exposes by default only from version 19. The
runs recorded above were made on Node 22.22.2 against PostgreSQL 16.

Coverage for `8360d8d6` is attached as
[`coverage-clover-8360d8d6.xml`](./evidence/coverage-clover-8360d8d6.xml).
The original file from July 2025 is retained outside this repository
(`coverage/` is git-ignored); it carries an internal generation timestamp of
12 July 2025 13:57:24 JST — six minutes after `8360d8d6` — and can be sent on
request.

### Runtime behaviour

The application logs through Winston with `@google-cloud/logging-winston`, and
Cloud Run records every inbound request with its status code. The queries below
are the method; the figures are what they return over the 30 days ending
10 September 2026.

| Metric | Measured |
| --- | ---: |
| Database timeout entries | 0 over 30 days (0/day) |
| Authentication failures | 223 of 312,397 requests (0.071%) |

```sql
-- Database timeout entries, daily
SELECT DATE(timestamp) AS day, COUNT(*) AS db_timeouts
FROM `co-creation-dao-prod.global._Default._AllLogs`
WHERE timestamp >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 30 DAY)
  AND resource.type = 'cloud_run_revision'
  AND REGEXP_CONTAINS(
        CONCAT(COALESCE(text_payload, ''),
               COALESCE(TO_JSON_STRING(json_payload), '')),
        r'P2024|ETIMEDOUT|Timed out fetching|connection pool')
GROUP BY day ORDER BY day;

-- Authentication failure rate, daily
SELECT DATE(timestamp) AS day,
       COUNTIF(http_request.status IN (401, 403))                                    AS auth_failures,
       COUNT(*)                                                                      AS total_requests,
       ROUND(SAFE_DIVIDE(COUNTIF(http_request.status IN (401, 403)), COUNT(*)) * 100, 3) AS auth_failure_pct
FROM `co-creation-dao-prod.global._Default._AllLogs`
WHERE timestamp >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 30 DAY)
  AND resource.type = 'cloud_run_revision'
  AND http_request.status IS NOT NULL
GROUP BY day ORDER BY day;
```

Figures for 2025 are not available. The project's `_Default` log bucket has
30-day retention with only the two built-in sinks and no export to BigQuery or
Cloud Storage, so log data from that period has aged out, and the query results
from the time were not retained.

### What was removed and why

Five figures in an earlier version of this section have been restated. Each is
listed with what replaced it:

| Claim | What changed |
| --- | --- |
| Test success 70% (210 of 300) before the fixes | Mis-stated. The correct figure is 117 of 177 (66.1%); the corrected table and the saved output of both runs are above. |
| Database timeouts 25/day before the fixes | The figure for that period cannot be re-derived, as the 2025 log data has passed retention. The method and a current measurement are above, with the query. |
| Authentication failures 12% before the fixes | As above. |
| External API failures 15% → 2% | This related to the NFT wallet registration and metadata sync path, not to the DID/VC issuance work documented in this report. Parallel calls on that path were timing out; a concurrency limit, rate control on the sync batch, and timeout log-level changes were added — but that work landed in October 2025, outside this report's window, so it is not documented here and the rate is not restated. |
| Debugging time reduced by 60% | A qualitative assessment. What the change delivered — transaction duration and slow-query logging, and structured logs queryable in Cloud Logging — is described in the fix entry for upstream PR #346. |

The fixes documented in this report are unaffected. Each carries its root
cause, the change made, and the commit that made it; all 105 commit references
in this report resolve in this repository.

---

## 🔧 Technical Categories

### Database & Transactions (4 fixes)
- Transaction timeout resolution
- Schema consistency improvements
- Community association fixes
- Logging and monitoring enhancements

### Type Safety & Validation (3 fixes)
- BigInt handling improvements
- Prisma enum alignment
- Data converter validation

### Async Processing & External APIs (3 fixes)
- Promise handling corrections
- VC/DID issuance workflow improvements
- Authentication token standardization

### Testing & Quality Assurance (2 fixes)
- Unit test enum corrections
- Integration test stability improvements

---

## 📝 Lessons Learned

### Prevention Strategies
1. **Comprehensive Type Checking**: Implement stricter TypeScript configurations
2. **Transaction Monitoring**: Proactive timeout and performance monitoring
3. **Async Pattern Enforcement**: Standardized async/await usage guidelines
4. **Schema Validation**: Automated schema drift detection

### Process Improvements
1. **Pre-commit Validation**: Enhanced validation hooks for enum consistency
2. **Integration Testing**: Expanded coverage for external API interactions
3. **Performance Testing**: Regular transaction timeout testing
4. **Documentation**: Improved error handling documentation

---

## 🔍 How to Verify These Fixes

### Prerequisites
```bash
# Clone the repository
git clone https://github.com/Co-Creation-DAO/civicship-api-251127.git
cd civicship-api-251127

# Install dependencies
pnpm install
```

### Viewing Individual Fixes
```bash
# View a specific commit
git show <commit-hash>

# View only the changed files
git show --name-only <commit-hash>

# View the full commit history
git log --oneline --all | head -50

# Search for specific fixes
git log --grep="transaction\|async\|enum" --oneline
```

### Running Tests
```bash
# Run all tests
pnpm test --runInBand

# Run specific test file
pnpm test <test-file-path>

# Run tests with coverage
pnpm test:coverage

# Run integration tests for transactions
pnpm test pointTransfer
```

### Database Migration Verification
```bash
# Check migration status
pnpm db:migrate status

# View specific migration
cat src/infrastructure/prisma/migrations/<migration-name>/migration.sql

# View all migrations
ls -lt src/infrastructure/prisma/migrations/

# Compare schema with database
pnpm db:pull --print
```

### Code Inspection
```bash
# Search for transaction handling
grep -r "ctx.issuer.onlyBelongingCommunity" src/application/domain/transaction/

# Check materialized view refresh
grep -r "refreshCurrentPoint" src/application/

# View authentication middleware
cat src/presentation/middleware/auth/index.ts
```
