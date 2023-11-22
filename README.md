# DNS Resolve

`dns-resolve` is a simple command-line DNS resolver written in Rust. It allows you to query a DNS server for the IP address associated with a given domain name.

## Usage

```bash
./dns-resolve [OPTIONS] <domain-name>
```

### Options

- `-s, --dns-server <dns-server>`: Specifies the DNS server to use for the query. Default is `1.1.1.1`.

### Example

```bash
./dns-resolve -s 8.8.8.8 example.com
```

## Dependencies

- [clap](https://crates.io/crates/clap): Command-line argument parsing.
- [rand](https://crates.io/crates/rand): Random number generation.
- [trust-dns](https://crates.io/crates/trust-dns): DNS library for Rust.

## Building

Make sure you have [Rust](https://www.rust-lang.org/tools/install) installed.

```bash
cargo build --release
```

## Running

```bash
cargo run -- [OPTIONS] <domain-name>
```
