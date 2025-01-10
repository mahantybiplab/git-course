<p>The <code>git push</code> command pushes (sends) local changes to any "remote" - in our case, GitHub. For example, to push our local <code>main</code> branch's commits to the remote <code>origin</code>'s <code>main</code> branch we would run:</p>

```bash
    git push origin main
```

### Alternative Options

You can also push a local branch to a remote with a different name:

```bash
    git push origin <localbranch>:<remotebranch>
```

It's less common to do this, but nice to know.

You can also delete a remote branch by pushing an empty branch to it:

```bash
    git push origin :<remotebranch>
```

