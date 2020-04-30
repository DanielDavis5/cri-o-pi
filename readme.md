# CRI-O-PI

Builds CRI-O using the Raspberry Pi toolchain.

## How to build

This example is for the Raspberry Pi 3 - Model B+.

    mkdir build
    ./src/prepare -C build
    ./src/build -C build arm 7

For instructions for other models use:

    ./src/build --help

### Installation

    cd build
    ./install

## Create a new release

    mkdir build
    ./src/prepare -C build
    ./src/build --release RELEASE_VERSION \
        --installer '../src/install.sh' \
        -C build arm 7
