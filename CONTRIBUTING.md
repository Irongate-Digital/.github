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

## Versioning & releases

Some repositories automate semantic versioning from Conventional Commits with
[release-please](https://github.com/google-github-actions/release-please-action). In those repos:

- **The pull request title drives the version bump** — squash-merge makes it the commit message
  that release-please reads. Keep it conventional: `feat(scope): ...`, `fix(scope): ...`, `chore(scope): ...`.
- Bump mapping:

  | Title prefix | Version | Use for |
  |---|---:|---|
  | `feat(...)` | minor | New user-facing feature |
  | `fix(...)` | patch | Bug fix |
  | `feat!` / `BREAKING CHANGE` | major | Breaking / incompatible change |
  | `chore`, `docs`, `refactor`, `ci`, `test`, `perf`, `style` | no bump | Maintenance & tooling |

- **Discipline**: reserve `feat`/`fix` for real product changes. Use `chore`/`refactor` for tooling,
  instrumentation, docs and CI — otherwise they bump the release version for no user value.
- When a `feat`/`fix` lands, release-please opens a release PR (`chore(main): release vX.Y.Z`). Merge
  it to create the git tag, update `CHANGELOG.md` and publish the GitHub Release. Every release stays
  reviewable.
- Treat the release-generated `CHANGELOG.md` as the source of truth; don't hand-edit versions.

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