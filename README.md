# rb

[![Build Status](https://travis-ci.com/klingtnet/rb.svg?token=drwE1YPs35oqracubtuf&branch=master)](https://travis-ci.com/klingtnet/rb)

A thread-safe fixed size circular (ring) buffer written in safe Rust.

## Features

- thread-safe
- blocking and non-blocking IO
- no unsafe blocks
- never under- or overflows

## Examples

```sh
cargo run --example saw
```

## Benchmark

The benchmarking feature needs *rust nightly*.

```sh
multirust run nightly -- cargo bench
```

It takes on my `Intel(R) Core(TM) i5-2520M CPU @ 2.50GHz` about `16ms` to push 2.8 million samples through the buffer in blocking IO mode.
