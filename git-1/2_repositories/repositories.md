<p>
    A file can be in one of
    <a
    href="https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#_the_very_basics"
    target="_blank"
    rel="noopener nofollow"
    >several states</a
    >
    in a Git repository. Here are a few important ones:
</p>
<ul>
    <li><code>untracked</code>: Not being tracked by Git</li>
    <li><code>staged</code>: Marked for inclusion in the next commit</li>
    <li><code>committed</code>: Saved to the repository's history</li>
</ul>
<p>
    The <code>git status</code> command shows you the current state of your
    repo. It will tell you which files are untracked, staged, and committed.
</p>

```bash
    git --no-pager log -n 10
```
