# NumPy - Xavier JP5

This repository anchors the numerical ABI for the Xavier Python 3.10 dependency stack. PyTorch-adjacent libraries, SciPy, scikit-image, scikit-learn, and the worker all depend on a compatible NumPy build.

## Role in the Xavier stack

- Provides the pinned AArch64 numerical base used by Worker v13.
- Prevents accidental ABI drift across locally built scientific wheels.
- Supports reproducible builds on Ubuntu 20.04.
- Remains API-compatible with the selected upstream release line.

## Project status

The selected build is part of an experimental whole-stack port. NumPy success alone does not prove the worker runtime.

## Build discipline

Native builds must use exactly one compiler worker.

## Upstream

Forked from `numpy/numpy`. This fork records Xavier build and compatibility work; upstream remains authoritative for NumPy itself.
