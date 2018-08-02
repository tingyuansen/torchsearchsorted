# Pytorch Custom CUDA kernel for searchsorted

This repository is an implementation of the searchsorted function to work for pytorch CUDA Tensors.

It is derived from the awesome [Pytorch Custom CUDA kernel Tutorial](https://github.com/chrischoy/pytorch-custom-cuda-tutorial)

**Disclaimer**

`This function has not been heavily tested. Use at your own risks`
## Description

Implements a function `searchsorted(a, v)` that works just like the [numpy version](https://docs.scipy.org/doc/numpy/reference/generated/numpy.searchsorted.html#numpy.searchsorted) except that `a` and `v` are assumed to be matrices of respective shape `(nrows, ncols_a)` and `(nrows, ncols_v)`.

the output is of the same size as `v`. Only works with pytorch tensors that are
already on the GPU.

## Installation

Just `make`


## Testing

Try `python test.py` with `torch` available. Tested on Pytorch v0.4.
