# git-wip

This is git stash, but branch-dependent.

- `wip "message"` — stash all changes for the current branch
- `wips` — list WIPs for the current branch
- `unwip` — restore the newest WIP for the current branch

WIPs are local Git stashes and are therefore never pushed.


# Installing

```
mkdir -p ~/.local/bin
chmod +x ~/.local/bin/wip

ln -sf ~/.local/bin/wip ~/.local/bin/wips
ln -sf ~/.local/bin/wip ~/.local/bin/unwip
``` 
