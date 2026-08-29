# Binary Ninja headless analysis with marimo

This repository contains a marimo notebook that uses the Binary Ninja Python
API outside the desktop UI.

## Requirements

- Binary Ninja with a license that permits headless API use
- Python 3.12
- [uv](https://docs.astral.sh/uv/)

Install Binary Ninja's Python API with the `install_api.py` script included in
your Binary Ninja installation before starting the notebook.

## Run the notebook

```bash
git clone https://github.com/meerkatone/binary_ninja_headless_and_marimo.git
cd binary_ninja_headless_and_marimo
uv venv --python 3.12
source .venv/bin/activate
python "/Applications/Binary Ninja.app/Contents/Resources/scripts/install_api.py"
uv pip install marimo
marimo edit binary_ninja_headless.py
```

The command above installs the Binary Ninja API into the active virtual
environment. Adjust the application path if you use a Personal, development,
non-default, or non-macOS installation.
