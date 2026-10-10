# Changelog

## Unreleased

- Ecosystem standardization: SECURITY.md, CONTRIBUTING.md, requirements, CI smoke checks.

## 1.0.0 (2026-09-18)

- Initial stable single-tool release (educational, authorized-use only).

## [3.0.0] - 2026-10-11
### Added
- 34 real modules (was 31 inflated with 3 duplicates + 2 print-only)
- Baseline request before injection tests; dual-math SSTI; error-based SQLi/LDAP/XPath with baseline guard
- Param discovery from actual URL (--param to force); JWT decode (alg/none/expiry); CNAME takeover via raw DNS
- HTTP methods, session cookie flags, secrets scan, GraphQL introspection, HPP delta, IDOR swap-diff
- Unified TBH v3 CLI: --proxy, --cookie, -H, --timeout, --json, --list, -m module selector
- Exit codes: 0 clean, 1 High/Medium finding, 2 error
### Fixed
- Bare except blocks everywhere; hardcoded ?q= params ignored real URL params; FP-prone single checks
