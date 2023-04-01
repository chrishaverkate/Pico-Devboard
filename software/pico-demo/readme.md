# Overview
A template for getting started with the Raspberry Pi Pico. 

This is a limited guide and assumes familiarity with:
* CMake
* C/C++
* Docker
* Raspberry Pi Pico

To learn more, there are plenty of guides, tutorials, and videos that do a much better
job than I can today.

## Features
* CMake build system
* CMake toolchain file for cross-compiling
* Docker container for cross-compiling
* Abstraction library to enable TDD on core logic
* Google Tests and Google Benchmark libraries setup with example
* A Pico related documents to get started

## Getting Started
This project is just a starting template and only tested on Linux. 
It's likely usable in WSL and on Mac (with some modification), but I haven't tested it.

_Note_, I've included some documents in the 'docs' folder, but it's always good
to check for updates.

### Prerequisites
* [Docker](https://docs.docker.com/get-docker/)
* [Pico Probe](https://www.raspberrypi.org/documentation/rp2040/getting-started/#debug-probe)
* [Raspberry Pi Pico](https://www.raspberrypi.org/products/raspberry-pi-pico/)
* [CMake](https://cmake.org/download/)
* Compiler tools for your platform

### Build - Local
To build locally, use the convenience script [run-build-linux.bash](scripts/run-build-linux.bash).
You can see the details of the build for setting up an IDE for more interactive development.
```bash
cd scripts && ./run-build-linux.bash linux
```

### Build - Docker
Again, there is a convenience script [run-build-docker.bash](scripts/run-build-docker.bash).
```bash
cd scripts && ./run-build-docker.bash
```

The benefit to this script is the output will be placed in the 'bin' folder,
and it will be ready to flash to the Pico.


