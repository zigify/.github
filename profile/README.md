# Zigify

*Target Zig Version: 0.13.0*

This organization serves to provide a centralized place to source C libraries with Zig build system compatibility as well as finding Zig wrappers to various C libraries. Every repository here uses [statically](https://github.com/zigify/statically), allowing for switching between static and dynamic compilation of the C dependencies.

## Libraries
| Name       | Build Support                                         | Wrapper |
| :--------: | :---------------------------------------------------: | :-----: |
| libusb     | [yes ✅](https://github.com/zigify/libusb-zys.git)    | 🛠️       |
| libftdi    | [yes ✅](https://github.com/zigify/libftdi-zys.git)   | 🛠️       |
| libyaml    | [yes ✅](https://github.com/zigify/libyaml-zys.git)   | 🛠️       |

## Adding/Requesting a Libary
You can open an issue [here](https://github.com/zigify/request) with whatever request you have! This can be as simple as asking for a library to be included or as involved as providing your own build support repo or wrapper.

## Repository Naming

### lib*-zys
Repositories with this name pattern are the raw C libraries with compatibility added to build them using Zig. These forks follow upstream with a `release-vX.Y.Z` branch following each release of the source library. These provide the raw C bindings for the library and can be accessed through `@cImport() and @cInclude()`.

### z-*
Repositories with this name pattern are the wrappers for the corresponding C library. These wrappers follow the upstream with a `release-vX.Y.Z` branch following each of the source library. These are still a work in progress.
