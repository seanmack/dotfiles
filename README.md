In `~/.bash_profile`:

```
for DOTFILE in `find "$HOME/dotfiles/bash"*`
do
  [ -f $DOTFILE ] && . "$DOTFILE"
done
```

---

In `~/.gitconfig`:

```
[include]
    path= dotfiles/git/gitconfig
```

---

Rename `~/.atom` to back it up, then tell Atom where to look for its config:

```
ln -s ~/dotfiles/atom ~/.atom
```

Then install `package-sync` package if you haven't already and run its "Sync" command.

---

In iTerm2 > Preferences > General > Preferences:

1.  Opt to load preferences from `~/dotfiles/iTerm2`

2.  Enable saving to folder on quit.
