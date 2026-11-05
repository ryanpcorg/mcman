# Security Policy

## Supported Versions

To ensure you are protected against known vulnerabilities, always run the latest stable release. We do not provide security patches or backports for older versions.

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |
| Older   | :x:                |

## Reporting a Vulnerability

**Do not open a public issue.** Public disclosure exposes all users to potential risk before a patch can be developed and deployed.

Please report all security vulnerabilities privately through GitHub's private vulnerability reporting feature:

1. Navigate to the repository's **Security** tab.
2. Select **Advisories** from the left-hand sidebar.
3. Click **Report a vulnerability** to open a draft advisory.

We will review your report, investigate the issue, and coordinate an advisory and release as quickly as possible.

## Out of Scope

- **Upstream / Third-Party Server JARs:** Do not report vulnerabilities found directly within third-party server `.jar` files (e.g., Paper, Spigot, Purpur). We do not develop or maintain these components and cannot remediate issues within upstream binaries. Please report those directly to the respective upstream maintainers.
