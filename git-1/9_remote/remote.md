### Adding a Remote

In git, another repo is called a "remote." The standard convention is that when you're treating the remote as the "authoritative source of truth" (such as GitHub) you would name it the "origin".

By "authoritative source of truth" we mean that it's the one you and your team treat as the "true" repo. It's the one that contains the most up-to-date version of the accepted code.

```bash
    git remote add <name> <uri>

    #inside webflyx-local directory
    git remote add origin ../webflyx
```

### Fetch

<p>Adding a remote to our Git repo does <em>not</em> mean that we automagically have all the contents of the remote. First, we need to <a href="https://git-scm.com/docs/git-fetch" target="_blank" rel="noopener nofollow">fetch</a> the contents (but not yet!).</p>

```bash
    git fetch
```

<p>This downloads copies of all the contents of the <code>.git/objects</code> directory (and other book-keeping information) from the remote repository into your current one.</p>

### Not Fetched

Just because we fetched all of the metadata from the remote <code>webflyx</code> repo doesn't mean we have all of the files.

### Log Remote

The git log command isn't only useful for your local repo. You can log the commits of a remote repo as well!

```bash
    git log remote/branch
    #  if you wanted to see the commits of a branch named primeagen from a remote named origin you would run:
    git log origin/primeagen

```

### Merge

Just as we merged branches within a single local repo, we can also merge branches between local and remote repos.


<p>For example, if you wanted to merge the <code>primeagen</code> branch of the remote <code>origin</code> into your local <code>main</code> branch, you would run this inside the local repo while on the <code>main</code> branch:</p>

```bash
    git merge origin/primeagen
```
