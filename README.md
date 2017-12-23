# vTerminal

A preservative fork of one of my new favorite new terminal emulators:
[Alacritty](https://github.com/jwilm/alacritty).

### Building

On macOS `10.13.1`:

```sh
git clone https://github.com/vvkmnn/vTerminal.git
curl -sSf https://static.rust-lang.org/rustup.sh | sh
cd vterminal
git pull remote upstream
cargo build --release
make app
cp -r target/release/osx/Alacritty.app /Applications/Alacritty.app
```

If all goes well, this should place a binary at `target/release/alacritty`.

### Setting

`alacritty.yml`, required in any of the following paths:

1. `$XDG_CONFIG_HOME/alacritty/alacritty.yml`
2. `$XDG_CONFIG_HOME/alacritty.yml`
3. `$HOME/.config/alacritty/alacritty.yml`
4. `$HOME/.alacritty.yml`

This one uses
[mine.](https://github.com/Vvkmnn/dotfiles/blob/master/.config/alacritty/alacritty.yml)
