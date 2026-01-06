# RailOS-Inno-Setup

This repository contains scripts for building setup executables for [Railway Operation Simulator](https://github.com/Railway-Op-Sim/railway-dot-exe) using Inno.

## Constraints

The installed program runs correctly only if installed in non administrative mode (for current user only). This is due to the fact that RailOS changes files within its program directory, which would require special permissions in case of the regular, system-wide `C:\Program Files\`. To avoid confusion and requiring Administrator permissions for regular use, the setup executable disables the system-wide option in the GUI installer.

## Updates

Whenever a new release of RailOS is published, the scripts have to be updated with the new version number before building the new setup executables. Please note the `MyAppVersion` value, but also any paths which include the version number, such as `LicenseFile` or the source entry under `[Files]`.

## Building

The scripts are best built and modified using the [Inno Setup Compiler](https://jrsoftware.org/isinfo.php) (building was done with the latest v6.6.1). RailOS program files should be placed in the same directory as the script before running.
