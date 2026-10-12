# Security Policy

## Reporting a vulnerability

**Please do not report security vulnerabilities in public GitHub issues.**

Instead, use GitHub's private vulnerability reporting: open the **Security**
tab of the affected repository (for example,
[`okforest/cli`](https://github.com/okforest/cli/security)) and click
**Report a vulnerability**. This opens a private advisory that only
maintainers can see.

If you can't use GitHub, email
[security@okforest.ai](mailto:security@okforest.ai).

We will acknowledge your report within 5 business days. Please give us a
reasonable window to ship a fix before disclosing publicly; we'll coordinate
disclosure with you once a fix is available.

## Supported versions

Security fixes are applied to the latest release of each open-source package
and action: the [`okforest`](https://www.npmjs.com/package/okforest) CLI,
[`@okforest/okf`](https://www.npmjs.com/package/@okforest/okf),
[`@okforest/validate`](https://www.npmjs.com/package/@okforest/validate), and
the OKForest Validate GitHub Action. Older releases are not patched; please
update to the latest version.

## Scope

**In scope**

- The open-source packages, GitHub Action, and Agent Skills published from
  the `okforest` GitHub organization.
- The hosted OKForest service at `okforest.ai` and its subdomains. Reports are
  welcome, but do not test against it without permission: no automated
  scanning, no denial of service, and no access to data that isn't yours.

**Out of scope**

- The Open Knowledge Format specification itself. Report issues with the
  format to the
  [upstream repository](https://github.com/GoogleCloudPlatform/open-knowledge-format).
- How an AI assistant or MCP client presents or acts on content it reads.
  Issues with a client's behavior belong with that client's vendor.
- Vulnerabilities in dependencies with no demonstrated impact on OKForest.
  Report those to the dependency's maintainers.
