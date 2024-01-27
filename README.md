# Rust learning 🦀️

## references

- https://github.com/rust-lang/rustlings
- https://doc.rust-lang.org/book/index.html

## ch01-01

### installation

- `curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh`
- get a C compiler on macOS `xcode-select --install`
- `rustc --version`
- `rustup update`

## ch01-02

### Hello, world!

create first Rust code by using `rustc` directly!

- `touch main.rs`

  - ```rust
      fn main() {
    	println!("Hello, world!");
    }
    ```

- `rustc ./main.rs`
- `run main`
  then print Hello, world!

`println!` calls a Rust macro

## ch01-03

### using Cargo

Cargo is Rust's build system and package manager

```sh
cargo new hello_cargo
```

generates 2 files:

- src/main.rc
- Cargo.toml (short for Tom's Obvious, Minimal Language which is Cargo's configuration format)
- `cargo new` will also initialize the git repository

### building and running a cargo project

- `cargo build` creates an executable file in `target/debug/hello_cargo`

  - run the executable `./target/debug/hello_cargo` -> print result

- `cargo run` compile the code and then run the resultant executable all in one command
- `cargo check` quickly checks your code to make sure it compiles but doesn’t produce an executable
- `cargo build --release` create an executable in target/release instead of target/debug
