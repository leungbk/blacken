# Blacken

Use the python `black` package to reformat your python buffers.

## usage

The whole buffer can be reformatted with `blacken-buffer`. If you want
to format every time you save, enable `blacken-mode` in relevant
python buffers. Note that if `blacken-only-if-project-is-blackened` is
non-nil, then blacken will only run if your `pyproject.toml` contains
the `[tool.black]` setting. This setting is off by default.


## customization

The following options change the behavior of black when reformatting buffers.

- `blacken-allow-py36` Allow using Python 3.6-only syntax on all input files.
- `blacken-skip-string-normalization` Don't normalize string quotes or prefixes.
- `blacken-fast-unsafe` Skips temporary sanity checks.
- `blacken-line-length` Max line length enforced by blacken.
