# container-template-lib
A library of container templates to enable reproducible containers for scientific computing

## Docs
Coming Soon...

## Base Templates
These currently exist in other repositories:
- [Docker Nix Base Template](https://github.com/XSEDE/docker-centos-nix-base) - The base Docker container for including the Nix package manager, based off of the original version developed at NixOS.
- [Singularity Nix Base Template](https://github.com/XSEDE/singularity-nix-base) - The base Singularity container (converted from the Docker container) for including the Nix package manager.
- [Docker Nix OpenMPI Base Template](https://github.com/XSEDE/docker-centos-nix-openmpi) - A Docker container with Nix to be used as a base template for applications using OpenMPI.
- [Singularity Nix OpenMPI Base Template](https://github.com/XSEDE/singularity-nix-openmpi) - A Singularity container (converted from the Docker container) to be used as a base template for applications using OpenMPI.  This also includes the Linpack HPL benchmark with a sample slurm job script for testing.
- [CUDA Base Template](https://github.com/XSEDE/nix-container-cuda-10.2) - Both a Docker and Singularity container with Nix for installing the CUDA 10.2 toolkit; to be used as a base template for GPU-oriented applications.
- [Python Base Template](https://github.com/XSEDE/nix-container-python) - Both a Docker and Singularity container with Nix for python3 to be used as a base template for python applications.

## Software Templates
These currently exist in other repositories:
- [sc-benchmark](https://github.com/XSEDE/nix-container-sc-benchmark) - Both a Docker and Singularity container with Nix for running the [sc-benchmark](https://github.com/FredHutch/sc-benchmark).  This includes setting up R and python using the Nix package manager, and can serve as a template for similar applications.
- [Python Mandle App](https://github.com/XSEDE/nix-container-python-mandle) - Both a Docker and Singularity container with Nix for a python3 application that allows you to create a GIF file with a straight-line zoom-in of the Mandlebrot set, based on the Python Base Template.
- [PerfZero](https://github.com/XSEDE/nix-container-perfzero) - Both a Docker and Singularity container with Nix for running the [Tensorflow PerfZero benchmarks](https://github.com/tensorflow/benchmarks/tree/master/perfzero) containing both Python and R dependencies.
