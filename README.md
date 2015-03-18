# Makefile.lammps.phpc
LAMMPS Makefile for PERSONALHPC machines 

This script does the following
- get latest openmpi sources from their git repo
- compile them to /opt/ompi
- get latest lammps sources from their git repo
- compile it to /opt/lammps/lammps

Just open a terminal and type :
```bash
wget 'https://raw.githubusercontent.com/personalhpc/LAMMPS-Makefile-for-PersonalHPC/master/script_compilation' && sh script_compilation
```
