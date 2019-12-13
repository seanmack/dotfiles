
Follow instructions for [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh). After downloading, it should boil down to the below:

1. `ln -s ~/dotfiles/zsh/.zshrc ~/.zshrc`

2. Set up syntax highlighting following the instructions [here](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md).

_Note: I've only recently switched to zsh, so the above steps are likely to be tweaked after I've had to set things up on another machine._

---

In `~/.gitconfig`:

```
[include]
    path= dotfiles/git/gitconfig
```

---

In iTerm2 > Preferences > General > Preferences:

1.  Opt to load preferences from `~/dotfiles/iTerm2`

2.  Enable saving to folder on quit.

---

Postgres

`ln -s ~/dotfiles/postgres/psqlrc ~/.psqlrc`
