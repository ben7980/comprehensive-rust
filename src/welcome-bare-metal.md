# Welcome to Bare Metal Rust

Today we will talk about 'bare-metal' Rust: running Rust code without an OS underneath us. This will
be divided into several parts:

 * What is `no_std` Rust?
 * Writing firmware for microcontrollers.
 * Writing bootloader / kernel code for application processors.
 * Some useful crates for bare-metal Rust development.

For the microcontroller part of the course we will use the [BBC micro:bit](https://microbit.org/) v2
as an example. It's a development board based on the Nordic nRF51822 microcontroller.

To get started, install some tools we'll need later:

```bash
sudo apt install gdb-multiarch picocom
rustup update
rustup target add thumbv7em-none-eabihf
cargo install cargo-binutils cargo-embed
```