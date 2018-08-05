### Readme

This repo contains a small bash script to install the netcdf-fortran libraries
and its dependencies. This may be useful when you are going to install
scicentifc models like WAVEWATCH III, WRF, SWAN, XBeach, GOTM, etc.

### Usage

To execute this script you simply type:

```
[sudo] CC=gcc FC=gfortran MAINDIR=/usr/local/netcdf ./install_netcdf.sh
```

where `CC` and `FC` are the path to C and Fortran compilers. If you want another
version of the dependencies you must edit the script manually.

