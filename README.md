# tide-tracing

[![License](https://img.shields.io/crates/l/tide_tracing.svg)](https://crates.io/crates/tide-tracing)
[![Latest version](https://img.shields.io/crates/v/tide-tracing.svg)](https://crates.io/crates/tide-tracing)
[![Latest Docs](https://docs.rs/tide-tracing/badge.svg)](https://docs.rs/tide-tracing/)
[![downloads-badge](https://img.shields.io/crates/d/tide_tracing.svg)](https://crates.io/crates/tide-tracing)

A simple middleware for [`tide`](https://github.com/http-rs/tide) using the [`tracing`](https://github.com/tokio-rs/tracing) crate for logging.

[![tide-tracing in action](/examples/example.png)](https://github.com/ethanboxx/tide-tracing/blob/master/examples/main.rs)

## Why

[`tide`](https://github.com/http-rs/tide) uses [`log`](https://github.com/rust-lang/log) in its [default logging middleware](https://docs.rs/tide/0.12.0/tide/log/struct.LogMiddleware.html).
When using [`tracing-log`](https://github.com/tokio-rs/tracing/tree/master/tracing-log) most of the information from tide is lost.
This crate provides a middleware that exposes all that information to [`tracing`](https://github.com/tokio-rs/tracing) directly while also improving the structure of the logs using [`span!`](https://docs.rs/tracing/0.1.17/tracing/span/index.html).

## Docs

- [API docs](https://docs.rs/tide-tracing/)
- [Example](https://github.com/ethanboxx/tide-tracing/blob/master/examples/main.rs)
