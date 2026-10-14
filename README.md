# MTPLX — shiftedx fork

Development fork of [youssofal/MTPLX](https://github.com/youssofal/MTPLX): local
inference on Apple Silicon using native multi-token prediction.

[Full reference](docs/REFERENCE.md) · [Quick start](docs/quickstart.md) · [Server guide](docs/server.md) · [Apache-2.0](LICENSE)

## Use upstream releases

For the maintained Mac app, downloads, and measured performance, use
[mtplx.com](https://mtplx.com) and [upstream releases](https://github.com/youssofal/MTPLX/releases).
PyPI and Homebrew install upstream packages, not this fork.

Requires Apple Silicon, macOS 14+, and Python 3.11+ for CLI development.
Model choice and memory requirements are in the [full reference](docs/REFERENCE.md#get-it).

## Work on this fork

```bash
git clone https://github.com/shiftedx/MTPLX.git
cd MTPLX
python3 -m venv .venv
. .venv/bin/activate
python -m pip install -e .
mtplx --help
```

Use a disposable environment; model weights download separately. Check the
[upstream comparison](https://github.com/youssofal/MTPLX/compare/main...shiftedx:MTPLX:main)
for the current fork delta before relying on a change.

## Reference

| Need | Guide |
| --- | --- |
| Models, installation, benchmarks | [Full reference](docs/REFERENCE.md) |
| Serve an API | [Server](docs/server.md) |
| CLI commands | [Quick start](docs/quickstart.md) |
| Development and tests | [Contributing](CONTRIBUTING.md) |
| Vulnerability reporting | [Security](SECURITY.md) |

Benchmark figures describe their recorded hardware and workloads; they are not
performance guarantees for this fork. Original attribution remains in [NOTICE](NOTICE).
