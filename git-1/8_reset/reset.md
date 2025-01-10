### Git Reset Soft

<p>The <a href="https://git-scm.com/docs/git-reset" target="_blank" rel="noopener nofollow">git reset</a> command can be used to undo the last commit(s) or any changes in the index (staged but not committed changes) and the worktree (unstaged and not committed changes).</p>

```bash
    git reset --soft COMMITHASH
```

<p>The <code>--soft</code> option is useful if you just want to go back to a previous commit, but keep all of your changes. Committed changes will be uncommitted and staged, while uncommitted changes will remain staged or unstaged as before.</p>

### Git Reset Hard

```bash
    git reset --hard COMMITHASH
```

This is useful if you just want to go back to a previous commit and discard all the changes.