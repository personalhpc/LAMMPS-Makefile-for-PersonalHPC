# Makefile.lammps.phpc

What this script does:
- get latest openmpi sources from their git repo
- compile them to /opt/ompi
- get latest lammps sources from their git repo
- compile it to /opt/lammps/lammps

Since it uses the /opt dir, it needs to be executed by a sudoer. It will ask for your sudo password once.
Good practice? NO! :)

Just open a terminal and type :
```bash
wget 'https://raw.githubusercontent.com/personalhpc/LAMMPS-Makefile-for-PersonalHPC/master/script_compilation' && sh script_compilation
```
