# Zellij tabs & status bar by (Alex Fedoseev)

This zellij tabs & status bar is made by [Alex Fedoseev](https://github.com/alex35mil) as a part of his [Dotfiles](https://github.com/alex35mil/dotfiles).

## Usage

Build it:

```bash
cargo build --release
```

Copy the `.wasm` file:

```bash
cp target/wasm32-wasi/release/zellij-bar.wasm ~/.config/zellij/plugins/
```

Add it to your layout:

```kdl
...
pane size=1 borderless=true {
    plugin location="file:~/.config/zellij/plugins/zellij-bar.wasm"
}
...
```
