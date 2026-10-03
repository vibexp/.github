# Security Policy

This policy applies to all repositories in the [`vibexp`](https://github.com/vibexp)
organization. It lives in the `.github` repository so it is inherited by every
repo that does not define its own `SECURITY.md`. A repository's own policy takes
precedence — [`vibexp/vibexp`](https://github.com/vibexp/vibexp/blob/main/SECURITY.md)
has one, covering supported versions and how fixes are released.

## Reporting a vulnerability

**Please do not open a public issue, discussion, or pull request for a security
problem.**

Report privately instead:

1. Go to the **Security** tab of the affected repository.
2. Click **Report a vulnerability**.
3. Describe what you found, the version or commit you tested, and how to
   reproduce it. A proof of concept helps, but a clear description is enough —
   do not delay a report to build one.

This opens a private advisory visible only to you and the maintainers. It is the
only reporting channel; there is no security mailing address to publish.

If the button is not visible to you, open a normal issue on the affected
repository saying **only** that you have a security report and would like a
private channel — no details — and a maintainer will open the advisory.

## What to expect

- **Acknowledgement.** A maintainer replies in the advisory thread confirming the
  report was received and whether it is reproducible.
- **A fix developed in private**, with the advisory published once a fixed
  release is available.
- **Credit**, unless you would rather stay anonymous — say so in the advisory.

These projects are maintained by volunteers, so please allow reasonable time for
a reply rather than a fixed SLA. If a report goes unanswered, a nudge in the
advisory thread is welcome.

## Scope

In scope: source code, CI/CD workflows, and published artifacts (container
images, packages, binaries) in `vibexp` repositories.

Out of scope: vulnerabilities in third-party dependencies with no
VibeXP-specific exploitation path (report those upstream), findings that require
an already compromised host or database, and self-inflicted misconfiguration of
a self-hosted instance.

## Leaked credentials

If you find a credential (API key, token, private key) committed to any
repository, treat it as live: report it privately as above and **do not** use it.
