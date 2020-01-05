# Dot Files

![](./images/dotfiles.png)

Image from https://github.com/jglovier

This directory holds useful dot file configurations.

[Dot files](https://medium.com/@webprolific/getting-started-with-dotfiles-43c3602fd789) are hidden on unix like systems (`Unix`, `Linux` and `Darwin/Mac` ).

Just copy&paste the relevant lines of the appropriate dotfile into your machine version.

## Terminals

There are two popular terminal programs:

- [Terminal](<https://en.wikipedia.org/wiki/Terminal_(macOS)>) (by default installed in MacOS)
- [iTerm2](https://iterm2.com/) (very popular open source terminal app)

## Shells

There are several varieties of shell programs. Two popular ones are:

- `zsh`

- `bash`

They are configured using hidden dot files stored in the users home directory.

(Type `echo $HOME` to see your home directory.)

### MacOS

zsh is now the [default on MacOS Catalina onwards](https://support.apple.com/en-us/HT208050)

### Terminal - bash: `.bashrc` and `.bash_profile`

If you use Terminal, then your default shell program is `bash`.

It is [recommended](https://scriptingosx.com/2017/04/about-bash_profile-and-bashrc-on-macos/) to use `.bashrc` for configurations and `.bash_profile` only loads `.bashrc`.

You could:

1. Make a `.bashrc` file in your home directory
   - either run `touch ~/.bashrc`
   - or save an empty file called `~/.bashrc` from your favorite text editor
2. Move the contents of your existing `~/.bash_profile` to `~/.bashrc`
3. Paste the contents of [`bash_profile`](./.bash_profile) to your now empty `~/.bash_profile`
   - this tell `~/.bash_profile` to load to `~/.bashrc`
4. Run the commands `chmod 700 ~/.bash_profile` and `chmod 700 ~/.bashrc`

Now you can copy&paste configurations from this repository's [`.bashrc`](./.bashrc) to your `.bashrc`

### iTerm - zsh: `.zshrc`

Some users may prefer to use the `z` shell that comes with the [iTerm2](https://iterm2.com/) program.

The environment for this is configured with `.zshrc`

Just copy&paste configurations from this repository's [`.zshrc`](./.zshrc) to your `.zshrc`
