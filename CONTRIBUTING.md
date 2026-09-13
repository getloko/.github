# Contributing to LoKO

Thanks for your interest in contributing! Here's how to get started.

## Repositories

Each part of the project lives in its own repo:

- **[loko](https://github.com/getloko/loko)** — Go CLI source (private repo, not open to external PRs)
- **[loko-releases](https://github.com/getloko/loko-releases)** — public binary releases; report CLI bugs here
- **[catalog](https://github.com/getloko/catalog)** — workload definitions
- **[getloko.github.io](https://github.com/getloko/getloko.github.io)** — documentation

## Reporting bugs

- **CLI bugs**: open an issue in [loko-releases](https://github.com/getloko/loko-releases) — the `loko` source repo is private
- **Workload/catalog bugs**: open an issue in [catalog](https://github.com/getloko/catalog)
- **Docs bugs**: open an issue in [getloko.github.io](https://github.com/getloko/getloko.github.io)

Include:
- Expected vs actual behavior

## Suggesting workloads

Open an issue in [catalog](https://github.com/getloko/catalog) with the workload name, Helm chart source, and a brief description of the use case.

## Pull requests

`catalog` and `getloko.github.io` are open to external PRs:

1. Fork the repository and create a branch from `main`
2. Follow the existing code style (YAML: match existing structure; Markdown: match existing structure)
3. Add or update tests if relevant
4. Open a PR — small, focused changes are easiest to review

`loko` (the CLI) is developed in a private repo; external code contributions aren't currently accepted there. File a bug in [loko-releases](https://github.com/getloko/loko-releases) instead.

## Development setup (CLI, internal contributors)

```bash
cd loko
make build      # dev binary
make test       # run unit suite
make lint       # go vet + golangci-lint
```

See the [loko Makefile](https://github.com/getloko/loko/blob/main/Makefile) for all targets.
