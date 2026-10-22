# Security Policy

This repository is the audit trail for the **2026 Q4 quarterly security review**. It records the security sweep performed across the account and the remediation work that follows from it.

## Reporting a Vulnerability

If you discover a security vulnerability in any repository covered by this policy:

1. **Do not open a public issue.** Public disclosure before a fix is in place puts users at risk.
2. Email the primary security contact: **Hezi Liu &lt;tackic@icloud.com&gt;** (contact details taken from the GitHub profile).
3. Include the repository name, the affected branch or commit, a description of the issue, and steps to reproduce it.
4. You will receive an acknowledgement within 3 business days, and a substantive response within 14 days.

## Scope of the 2026 Q4 Audit

This policy was published as part of the quarterly security review, which covered:

- **Account-wide code-scanning sweep** — every repository owned by `@HeziLiu` (Little-rookie, Big-Buzzard, CodingInterviewChinese2, awesome-chatgpt-prompts-zh) was checked for open code-scanning alerts. The code-scanning API returned `403 Resource not accessible by personal access token` for all four repositories, so no per-repository alert counts could be retrieved programmatically. Closing this gap requires a token with the `security_events` scope and is tracked in the "Enable code scanning baseline" sub-issue.
- **Organization-level repository security advisories** — the organization reachable from this account (`mcpmark-eval-liuhezi`) was checked for repository security advisories on record. The org-level advisory endpoint returned `403 Resource not accessible by personal access token`; a repo-level spot-check of this tracker repository returned zero advisories.
- **Remediation tracking** — the parent tracker issue "Security audit 2026 Q4 tracker" with three attached sub-issues: "Publish SECURITY.md policy", "Enable code scanning baseline", and "Document incident response runbook".

## Supported Versions

This repository is a tracker rather than a shipped product. The policy applies to the default branch (`main`) at all times.

## Contact

- Security contact: Hezi Liu — tackic@icloud.com
