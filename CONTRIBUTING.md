# Contributing to LoKO

Thanks for your interest in contributing! Here's how to get started.

## Repositories

Each part of the project lives in its own repo:

- **[loko](https://github.com/getloko/loko)** — Python CLI
- **[catalog](https://github.com/getloko/catalog)** — workload definitions
- **[getloko.github.io](https://github.com/getloko/getloko.github.io)** — documentation

## Reporting bugs

Open an issue in the relevant repository. Include:
- Your OS and `loko --version` output
- Steps to reproduce
- Expected vs actual behavior

## Suggesting workloads

Open an issue in [catalog](https://github.com/getloko/catalog) with the workload name, Helm chart source, and a brief description of the use case.

## Pull requests

1. Fork the repository and create a branch from `main`
2. Follow the existing code style (Python: ruff + mypy strict; YAML: match existing structure)
3. Add or update tests if relevant
4. Open a PR — small, focused changes are easiest to review

## Development setup (CLI)

```bash
cd loko
uv sync
poe test        # run unit tests
poe lint        # ruff check
poe typecheck   # mypy
```

See the [loko README](https://github.com/getloko/loko) for full setup instructions.
