[![Run script](https://github.com/dspelaez/install-netcdf-fortran/actions/workflows/run.yml/badge.svg)](https://github.com/dspelaez/install-netcdf-fortran/actions/workflows/run.yml)

### Readme

This repo contains a small bash script to install the netcdf-fortran libraries
and its dependencies. This may be useful when you are going to install
scientific models like WAVEWATCH III, WRF, SWAN, XBeach, GOTM, etc.

### Usage

To execute this script you must type:

```
[sudo] CC=gcc FC=gfortran MAINDIR=/usr/local/netcdf ./install_netcdf.sh
```

where `CC` and `FC` are the path to C and Fortran compilers and `MAINDIR` is the
prefix where the libraries are going to be installed. By default the C and
Fortran compilers are set to `CC=/usr/bin/gcc` and `FC=/usr/bin/gfortran`. The
default prefix is `MAINDIR=/usr/local/netcdf`.

NOTE: If you want another version of the dependencies you must edit the script
manually.


### Clean

To clean the installation you should remove the tar files

```
rm -f *.tar *.tar.gz
```
