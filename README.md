# Python interface for ænet

## Prerequisites

- aenet version 2.0.3 or greater
- Python 3.6+
- Cython

## Installation

(1) Compile the symmetry function C library. Within the `src` of the `aenet` installation directory, run

    $ cd ../src
    $ make -f ./makefiles/Makefile.XXX lib
    $ cd -

Select the Makefile.XXX that is appropriate for your system, but make sure to compile a serial version of `aenet`.

(2) Build Python extension module

    $ python setup.py build_ext --inplace
