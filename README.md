# git-wip

This is git stash, but branch-dependent.

- `wip "message"` — stash all changes for the current branch. `message` is optional.
- `unwip` — restore the newest WIP for the current branch. If you have local changes, the WIP is merged on top (conflict markers where both touch the same lines).
- `wips` — list all branches with WIPs and their WIP count
- `wips -d` / `wips --delete` — delete all WIPs of the current branch
- `-h`, `--help` on any of them — show usage

WIPs are local Git stashes and are therefore never pushed.


# Installing

Run from the repo directory:

```
mkdir -p ~/.local/bin
chmod +x wip
ln -sf "$PWD/wip" ~/.local/bin/wip

ln -sf ~/.local/bin/wip ~/.local/bin/wips
ln -sf ~/.local/bin/wip ~/.local/bin/unwip
``` 
