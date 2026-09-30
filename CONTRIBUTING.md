# Contributing

Thanks for contributing to an Irongate Digital repository.

## Before you start

- Open an issue first for anything larger than a trivial fix, so we can agree on the approach.
- Never commit secrets, credentials, customer data or real subscriber numbers (MSISDN). Use
  dummy values in code, tests and examples.

## Branching

- Branch from the repository's default branch (`master` or `main`).
- Use a descriptive, prefixed branch name:
  - `feat/<short-description>`
  - `fix/<short-description>`
  - `chore/<short-description>`
  - `docs/<short-description>`

## Commits

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

Common types: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `ci`, `perf`.

## Pull requests

- Keep pull requests small and focused; one concern per PR.
- Fill in the pull request template.
- Ensure CI is green before requesting review — tests, lint and build must pass.
- Request review from a code owner. Do not merge your own PR without review unless the
  repository explicitly allows it.
- Delete the branch after merge (configured automatically).

## Dependencies

- Dependency updates are proposed automatically by Dependabot (weekly) and scanned by
  Socket.dev on every pull request.
- Do not merge a dependency bump that breaks CI. For a major bump, read the upstream release
  notes first.

## Security

See [SECURITY.md](SECURITY.md) for how to report a vulnerability. Never open a public issue
for a security problem.

## Code of conduct

Participation in these repositories is covered by our
[Code of Conduct](CODE_OF_CONDUCT.md).