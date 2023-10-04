<p align="center">
  <img src="https://raw.githubusercontent.com/yetinam/pyocto/main/docs/_static/pyocto_logo_outlined.svg" />
</p>

[![PyPI - License](https://img.shields.io/pypi/l/pyocto)](https://github.com/yetinam/pyocto/blob/main/LICENSE)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/yetinam/pyocto/lint_and_test.yml?branch=main)](https://github.com/yetinam/pyocto)
[![Read the Docs](https://img.shields.io/readthedocs/pyocto)](https://pyocto.readthedocs.io/en/latest/)
[![PyPI](https://img.shields.io/pypi/v/pyocto)](https://pypi.org/project/pyocto/)
[![Python 3.9](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
[![DOI](https://zenodo.org/badge/DOI/xyz)](https://doi.org/xyz)

PyOcto is a high-throughput seismic phase associator.
The best way to get started with PyOcto is through our interactive example.
If you're looking for further guidance, for example, a guide on how to set
the associator parameters, check out the [PyOcto documentation](https://pyocto.readthedocs.org/).

## Installation

The easiest way to install PyOcto is through pip:

```bash
pip install pyocto
```

There are prebuilt wheels available for Linux, Mac OS, and Windows.
In case you want to use 1D velocity models, you will need to install
the optional dependency [pyrocko](https://pyrocko.org/). pyrocko is available through the
standard channels, such as `pip` or `conda`.

```bash
git clone https://github.com/yetinam/pyocto.git
cd pyocto
git submodule update --init
pip install .[test]
```

To verify your installation is working, use `pytest tests/`.

**Warning:** PyOcto uses POSIX threads for threading. As these are not available on Windows,
the Windows version is single-threaded. Therefore, we do not recommend running larger computations
on Windows.

## References
If you're using PyOcto in your work, please cite:

Münchmeyer, J. (2023). PyOcto: A high-throughput seismic phase associator. *arxiv preprint*
