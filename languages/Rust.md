# Rust

## Repository

<https://github.com/graalvm/sulong>

## Installation

LLVM runtime support comes built in with Graal.
Rust needs to be installed separately <https://rustup.rs>.

## Runs on Graal

:ballot_box_with_check: Yes

```shell
rustc --emit=llvm-bc hello-rust.rs
lli --lib $(rustc --print sysroot)/lib/libstd-* hello-rust.bc
```

## Supports Polyglot

:no_entry: Not supported
