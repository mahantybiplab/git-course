```bash
    git --no-pager log --oneline --decorate --graph --parents
```

<p style="font-size:18px">Fast Forward Merge</p>

<pre><code>      C     delete_vscode
     /
A - B       main
</code></pre>

And we run this while on <code>main</code>:
```bash
    git merge delete_vscode
```

Because <code>delete_vscode</code> has all the commits that <code>main</code> has, Git automatically does a fast-forward merge. It just moves the pointer of the "base" branch to the tip of the "feature" branch:

<pre><code>            delete_vscode
A - B - C   main
</code></pre>

<p>Notice that with a fast-forward merge, <strong>no <a href="https://git-scm.com/docs/git-merge#_true_merge" target="_blank" rel="noopener nofollow">merge commit</a> is created</strong>.</p>

