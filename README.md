# Container Template Library (CTL) Project Overview
The XSEDE Cyberinfrastructure Resource Integration (XCRI) team has developed the Container Template Library (CTL) which spans several repositories and purposes, 
all focused on containers for scientific computing.  The main goal of the CTL project is to collect a library of templates for scientific computing software containers that can be provided by cluster admins, run directly by users, edited by developers to create new scientific software containers, and used by anyone for learning how to build, develop, deploy, and run containers on XSEDE resources and XSEDE-like campus clusters.

## Project Goals & Products
This project is currently in-progress, so you can expect updates and changes here until completion.  In the meantime, this list includes both in-progress and completed items:

* A [Library](#Library) of container templates for scientific computing.
* There are several container templates that focus on reproducible builds by leveraging the Nix package manager features.
* We are developing robust testing of the containers on a variety of XSEDE systems using INCA to enable sysadmins and users to feel confident using these containers on their systems.
* We are integrating this work with the [Container Tutorial](https://github.com/XSEDE/Container_Tutorial) we have been providing to create a Learning Toolkit that people from a variety of backgrounds can start with to engage with containers for scientific computing.

## Questions & Contributing
If you have questions, comments, or suggestions, please feel free to open a new issue or pull request on this repository or send an email to `help@xsede.org` with **XCRI** in the subject line.

## Docs
Coming Soon...

# Library
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
- [NAMD2.14](https://github.com/XSEDE/nix-container-namd2.14-cuda10.2) - Both a Docker and Singularity container with Nix for running [NAMD2.14](https://www.ks.uiuc.edu/Research/namd/).
