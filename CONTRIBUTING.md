# Contributing

Thanks for helping grow OKForest. This is the default guide for every
repository in the organization; a repository's own `CONTRIBUTING.md` or
`AGENTS.md` adds its specifics (setup, tests, release steps).

## Before you start

- For anything bigger than a small fix, open an issue first so we can agree on
  the approach before you spend time on it.
- Security problems go through the [security policy](./SECURITY.md), never a
  public issue.
- Questions about the Open Knowledge Format itself (what a field means, a
  proposed change to the format) belong in the
  [upstream OKF repository](https://github.com/GoogleCloudPlatform/open-knowledge-format).
  OKForest follows the spec closely but does not own it.

## Making a change

- Use [Conventional Commits](https://www.conventionalcommits.org/) for commit
  messages and pull request titles (`feat:`, `fix:`, `docs:`, `chore:`, ...).
- Keep pull requests small and focused on one intent.
- In the TypeScript repositories, all four gates must pass before a pull
  request: `pnpm build && pnpm test && pnpm typecheck && pnpm check`. CI runs
  the same commands.
- Include a changeset (`pnpm changeset`) with any change that should ship in
  a published package.
- Add or update tests for behavior you change.

## Example data

Examples, fixtures, templates, and documentation must never use real
organizations or people as if they were users or publishers:

- Domains and email addresses: only reserved example domains, such as
  `acme.example`, `example.com`, `example.org`, or `example.net`.
- Names: generic placeholders such as "Acme", "Rival Co", "ExampleCRM", or
  "Jane".

Public sample content from elsewhere (for example, Google's OKF sample
bundles) keeps its original license and attribution.

## License

By contributing, you agree that your contributions are licensed under the
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), the same
license that covers the project (inbound = outbound). Contributing does not
grant rights to the OKForest name or logo; see the
[trademark policy](./TRADEMARKS.md).
