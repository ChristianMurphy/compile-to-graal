# Rust

## Repository

<https://github.com/graalvm/sulong>

<https://www.rust-lang.org>

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

:grey_question: Unknown

## Sources and Resources

- <https://www.graalvm.org/docs/reference-manual/languages/llvm/#running-rust>
