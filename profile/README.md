# Irongate Digital Solution Ltd

Backend, API and integration platform for prepaid top-up, game top-up and payment
distribution.

## What lives here

| Repository | Purpose |
| --- | --- |
| `cms` | Content management / admin back office |
| `prt` | Production application (top-up distribution) |
| `irongate-prepaid` | Prepaid product and transaction services |
| `irongate-developer` | Developer portal |
| `irongate-api-docs` | Public API documentation |
| `irongatedigital-landing` | Marketing site |
| `internal-go` | Internal Go services |
| `browser-service` | Browser automation service |
| `product-catalog-scraper` | Product catalogue ingestion |
| `ops-agent` | Operational gateway |
| `idsl-ui` | Shared UI library |

## Engineering standards

Every repository in this organisation follows the same baseline:

- **Dependency updates** — Dependabot, weekly, grouped minor/patch; alerts and security
  updates enabled.
- **Supply-chain scanning** — Socket.dev on every pull request.
- **CI** — tests, lint and build must pass before merge.
- **Least privilege** — workflows declare explicit, minimal `GITHUB_TOKEN` permissions.
- **Conventional Commits** and focused pull requests.

## Contributing

See [CONTRIBUTING.md](https://github.com/Irongate-Digital/.github/blob/main/CONTRIBUTING.md).

## Security

Report vulnerabilities privately — see [SECURITY.md](https://github.com/Irongate-Digital/.github/blob/main/SECURITY.md).
Please do not open a public issue for a security problem.

## Contact

- **General / support:** techsupport@irongatedigital.com
- **Engineering:** tech@irongatedigital.com