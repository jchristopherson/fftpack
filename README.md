![FFTPACK](media/logo-text-background.png)

# FFTPACK

A package of Fortran subprograms for the fast Fourier transform of periodic and other symmetric sequences.

[![Actions Status](https://github.com/fortran-lang/fftpack/workflows/fpm/badge.svg)](https://github.com/fortran-lang/fftpack/actions)
[![Actions Status](https://github.com/fortran-lang/fftpack/workflows/doc-deployment/badge.svg)](https://github.com/fortran-lang/fftpack/actions)
[![CMake](https://github.com/fortran-lang/fftpack/actions/workflows/cmake.yml/badge.svg?branch=main)](https://github.com/fortran-lang/fftpack/actions/workflows/cmake.yml)

## Getting started
### Get the code
```bash
git clone https://github.com/fortran-lang/fftpack.git
cd fftpack
```

### Build with [fortran-lang/fpm](https://github.com/fortran-lang/fpm)
Fortran Package Manager (fpm) is a package manager and build system for Fortran.   
You can build using provided `fpm.toml`:
```bash
fpm build
fpm test --list
fpm test <test_name, see `fpm.toml` or list>
```
To use `fftpack` within your `fpm` project, add the following to your `fpm.toml` file:
```toml
[dependencies]
fftpack = { git="https://github.com/fortran-lang/fftpack.git" }
```

## Build with Make
Alternatively, you can build using provided `Makefile`:
```bash
make
```

## Build with CMake
This library can also be built using CMake.  For instructions see [Running CMake](https://cmake.org/runningcmake/).  CMake version 3.24 or higher is required.

## Links
- [netlib/dfftpack1.0(fftpack4.0)](http://www.netlib.org/fftpack/)
- [Documents of fft routines in GNU/gsl based on `netlib/fftpack`](https://www.gnu.org/software/gsl/doc/html/fft.html#)
- [Documents of scipy.fftpack](https://docs.scipy.org/doc/scipy/reference/fftpack.html)
- [NACR/FFTPACK 5.1](https://www2.cisl.ucar.edu/resources/legacy/fft5)
