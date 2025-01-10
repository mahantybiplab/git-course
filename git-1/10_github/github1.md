```bash
    curl -sS https://webi.sh/gh | sh
    gh auth login
```

Navigate back into your <code>webflyx</code> repo locally, it's going to be our "local" repo

<label><a href="https://git-scm.com/docs/git-remote" target="_blank">Add a remote</a> to your <code>webflyx</code> repo that points to the <code>webflyx-remote</code> repo you just created. That command should look something like this:</label>

```bash
    git remote add origin https://github.com/your-username/webflyx.git
```
Run <code>git ls-remote</code> to make sure the remote was added correctly.

