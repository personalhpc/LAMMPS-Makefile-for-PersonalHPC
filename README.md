# LAMMPS @ PersonalHPC (PHPC)

## Preamble
This script is aimed at installing the very last vertion of [LAMMPS](http://lammps.sandia.gov/) on [PersonalHPC computers](www.personalhpc.com). It should be valid on any linux and iOS systems, but we did not test.
This script comes without any warranty.

## Licence
The MIT Licence applies. See accompagning LICENCE file.

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
## And then? How to use this brand new LAMMPS?

You should type in a terminal:
```bash
/opt/ompi/bin/mpirun -np 64 /opt/lammps/lammps < inputfile
```
where 64 is the number of cpu you want for your calculation.
You may add an alias for `/opt/ompi/bin/mpirun`, as long as it is not `mpirun`
You may add an alias for `/opt/lammps/lammps`, as long as it is not `lammps`
Why not `mpirun-phpc` and `lammps-phpc`, or `mpirun-1.9.0a1` and 
That's up to you, and more information can be found [here](http://community.linuxmint.com/tutorial/view/891)
