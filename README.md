In `~/.bash_profile`:

```
for DOTFILE in `find "$HOME/config/bash"*`
do
  [ -f $DOTFILE ] && . "$DOTFILE"
done
```

In `~/.gitconfig`:

```
[include]
    path= config/git/gitconfig
```

Tell Atom where to look for its config:

```
ln -s ~/config/atom ~/.atom
```
