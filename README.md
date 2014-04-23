# Private Collection of Dotfiles

This repository contains a selection of dotfiles with functionality to beef up the shell.

### How to install

1. Copy dotfiles to your home-directory

2. Add snippet to .bash_profile to load additional dotfiles

```bash
# Load given list of files from home-directory
for file in ~/.{aliases,functions}; do
  [ -r "$file" ] && source "$file"
done
unset file
```

Inspired by:
* Addy Osmani: [https://github.com/addyosmani/dotfiles]