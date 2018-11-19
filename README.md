In `~/.bash_profile`:

```
for DOTFILE in `find "$HOME/dotfiles/bash"*`
do
  [ -f $DOTFILE ] && . "$DOTFILE"
done
```

In `~/.gitconfig`:

```
[include]
    path= dotfiles/git/gitconfig
```

Tell Atom where to look for its config:

```
ln -s ~/dotfiles/atom ~/.atom
```
