### Rebase vs. Merge

I've configured Git to rebase by default on pull, rather than merge so I keep a linear history. If you want to do the same, you can add this to your global Git config:

```bash
    git config --global pull.rebase true
```

