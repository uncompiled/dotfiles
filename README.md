# dotfiles

These are my configs.

## Getting Started

### Components

Special files in the hierarchy:

- **Brewfile**: This is a list of applications for [Homebrew Cask](http://caskroom.io) to install: things like Chrome and 1Password and Adium and stuff. Might want to edit this file before running any initial setup.
- **topic/\*.zsh**: Any files ending in `.zsh` get loaded into your
  environment.
- **topic/path.zsh**: Any file named `path.zsh` is loaded first and is
  expected to setup `$PATH` or similar.
- **topic/completion.zsh**: Any file named `completion.zsh` is loaded
  last and is expected to setup autocomplete.
- **topic/install.sh**: Any file named `install.sh` is executed when you run [script/install](script/install). To avoid being loaded automatically, its extension is `.sh`, not `.zsh`.
- **topic/\*.symlink**: Any file ending in `*.symlink` gets symlinked into
  your `$HOME`. This is so you can keep all of those versioned in your dotfiles
  but still keep those autoloaded files in your home directory. These get
  symlinked in when you run [script/bootstrap](script/bootstrap).

### Setup

- `git clone https://github.com/uncompiled/dotfiles.git ~/.dotfiles`
- `cd ~/.dotfiles`
- `install && bootstrap`

This will symlink the appropriate files in `.dotfiles` to your home directory.
Everything is configured and tweaked within `~/.dotfiles`.

### Color Scheme

I like [Material Shell](https://github.com/carloscuesta/materialshell).

## Credits

These are based on @holman's [dotfiles](https://github.com/holman/dotfiles.git).
My dotfiles were getting unwieldy and I like the topic-based organization.
