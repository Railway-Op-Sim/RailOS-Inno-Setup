# RailOS-Inno-Setup

This repository contains scripts for building setup executables for [Railway Operation Simulator](https://github.com/Railway-Op-Sim/railway-dot-exe) using Inno.

## Constraints

The installed program runs correctly only if installed in non administrative mode (for current user only). This is due to the fact that RailOS changes files within its program directory, which would require special permissions in case of the regular, system-wide `C:\Program Files\`. To avoid confusion and requiring Administrator permissions for regular use, the setup executable disables the system-wide option in the GUI installer.

## Building

The scripts require the Inno Setup Compiler. RailOS program files should be placed in the same directory as the script before running.
