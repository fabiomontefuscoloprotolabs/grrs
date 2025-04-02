# grrs - A Rust CLI Search Tool

This is a learning project based on the [Command Line Applications in Rust](https://rust-cli.github.io/book/tutorial/) tutorial. The project implements a simple grep-like command-line tool that searches for a pattern in a file.

## Project Overview

`grrs` (pronounced "grass") is a simple CLI tool that:
- Takes a pattern and a file path as command-line arguments
- Searches for the pattern in the specified file
- Prints each line that contains the pattern

This project demonstrates:
- Command-line argument parsing with `clap`
- File I/O operations in Rust
- Error handling with the `Result` type
- Structuring a Rust CLI application

## Building and Running

### Using Cargo

```bash
# Build the project
cargo build

# Run the project (replace PATTERN and PATH with your values)
cargo run -- PATTERN PATH
```

### Using podman or docker

```bash
# Build the project
podman run -v$PWD:/app:z -w/app --rm rust cargo build

# Run the project (replace PATTERN and PATH with your values)
podman run -v$PWD:/app:z -w/app --rm rust cargo run -- PATTERN PATH
```
