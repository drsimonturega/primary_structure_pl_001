# NWChem install

export NWCHEM_TOP=/home/simon/nwchem/nwchem-7.2.2/
export NWCHEM_TARGET=LINUX64
export BUILD_OPENBLAS=1
export BUILD_SCALAPACK=1
export BLAS_SIZE=4
export SCALAPACK_SIZE=4
export USE_MPI=y
export USE_PYTHONCONFIG=y
export PYTHONVERSION=3.6
export PYTHONHOME=/usr/bin/python3.6
export USE_64TO32=y
export ELPA="-I/usr/lib64/gfortran/modules/openmpi -L/usr/lib64/openmpi/lib -lelpa"
export LD_LIBRARY_PATH=/usr/lib64/openmpi/lib/:$LD_LIBRARY_PATH
export PATH=/usr/lib64/openmpi/bin/:$PATH
