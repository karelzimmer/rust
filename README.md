# rust

Mijn Rust-programma's.
Voor (zelf)studie. Werk in uitvoering.

## Werkwijze Hello, world

```console
cd ~/rust
mkdir hello_world
cd hello_world
```

Edit main.rs:

```rust
fn main() {
    println!("Hello, world!");
}
```

Compile:

```console
rustc main.rs
```

Run:

```console
./main
```

Output:

```console
Hello, world!
```

## Werkwijze Hello, Cargo

```console
cd ~/rust
cargo new hello_cargo
```

Output:

```console
     Created binary (application) `hello_cargo` package
```

```console
cd hello_cargo
```

Generated Cargo.toml:

```rust
[package]
name = "hello_cargo"
version = "0.1.0"
edition = "2021"

[dependencies]
```

Generated src/main.rs:

```rust
fn main() {
    println!("Hello, world!");
}
```

Build:

```console
cargo build
```

```console
Output:
   Compiling hello_cargo v0.1.0 (/home/karel/rust/hello_cargo)
    Finished dev [unoptimized + debuginfo] target(s) in 2.35s
```

Run method 1:

```console
./target/debug/hello_cargo
```

Output:

```console
Hello, world!
```

Run method 2:

```console
cargo run
```

Output:

```console
    Finished dev [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/hello_cargo`
Hello, world!
```

Check code:

```console
cargo check
```

Output:

```console
    Checking hello_cargo v0.1.0 (/home/karel/rust/hello_cargo)
    Finished dev [unoptimized + debuginfo] target(s) in 0.09s
```
