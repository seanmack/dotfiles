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

In Atom, install `package-sync` package.

Rename `~/.atom` to back it up, then tell Atom where to look for its config:

```
ln -s ~/dotfiles/atom ~/.atom
```

Run the "Sync" command for `package-sync`.

---

In iTerm2 > Preferences > General > Preferences:

1.  Opt to load preferences from `~/dotfiles/iTerm2`

2.  Enable saving to folder on quit.

---

Postgres

`ln -s ~/dotfiles/postgres/psqlrc ~/.psqlrc`

---

TODO:

- Simplify setup

- Add a command to list all aliases
