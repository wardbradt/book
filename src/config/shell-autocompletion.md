## Shell Autocompletion

You can generate autocompletion shell scripts for `bash`, `elvish`, `fish`, `powershell`, and `zsh`.

### zsh

First, ensure that the following is present somewhere in your `~/.zshrc` file (if not, add it):

```sh
autoload -U compinit
compinit -i
```

Then run:

```sh
forge completions zsh > /usr/local/share/zsh/site-functions/_forge
cast completions zsh > /usr/local/share/zsh/site-functions/_cast
```

### fish

```sh
mkdir -p $HOME/.config/fish/completions
forge completions fish > $HOME/.config/fish/completions/forge.fish
cast completions fish > $HOME/.config/fish/completions/cast.fish
source $HOME/.config/fish/config.fish
```
