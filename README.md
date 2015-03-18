# LAMMPS @ PersonalHPC (PHPC)

## Preamble
This script is aimed at installing the very last vertion of [LAMMPS](http://lammps.sandia.gov/) on [PersonalHPC computers](www.personalhpc.com). It should be valid on any linux and iOS systems, but we did not test.
This script comes without any warranty.

## Licence
It's GPL. See accompagning LICENCE file.

## What this script does:
- get latest openmpi sources from their git repo
- compile them to /opt/ompi
- get latest lammps sources from their git repo
- compile it to /opt/lammps/lammps

Since it uses the /opt dir, it needs to be executed by a sudoer. It will ask for your sudo password once.
Good practice? NO! :)

## How-to

Open a terminal and type :
```bash
wget 'https://raw.githubusercontent.com/personalhpc/LAMMPS-Makefile-for-PersonalHPC/master/script_compilation' && sh script_compilation
```
