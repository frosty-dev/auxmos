Rust-based atmospherics for Space Station 13 using [auxtools](https://github.com/willox/auxtools).

The compiled binary on Citadel is compiled for Citadel's CPU, which therefore means that it uses [AVX2 fused-multiply-accumulate](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions#Advanced_Vector_Extensions_2). Yes, really. If you have issues, compile it yourself, via `cargo rustc --target=i686-pc-windows-msvc --release --features "all_reaction_hooks" -- -C target-cpu=native`. It has to be 32-bit, mind.

This code relies on some byond code on [this fork of Citadel](https://github.com/Putnam3145/Citadel-Station-13/tree/auxtools-atmos). Documentation on this is associated with the individual data structures that hold them, in this repository.

The compiled binary on Citadel is compiled for Citadel's CPU, which therefore means that it uses [AVX2 fused-multiply-accumulate](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions#Advanced_Vector_Extensions_2). Yes, really. If you have issues, compile it yourself, via `cargo rustc --target=i686-pc-windows-msvc --release --features "all_reaction_hooks" -- -C target-cpu=native`.

TODO:
I would quite a lot like monstermos to work.

