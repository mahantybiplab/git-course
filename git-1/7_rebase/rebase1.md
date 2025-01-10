<details open="">
<summary>
<h2>Visualizing Rebase</h2>
</summary>
<p>Say we have this commit history:</p>

<div>
	<pre><code>A - B - C    main
   \
    D - E    feature_branch
</code></pre>

</div>
<p>We're working on <code>feature_branch</code>, and want to bring in the changes our team added to <code>main</code> so we're not working with a stale branch. We could merge <code>main</code> into <code>feature_branch</code>, but that would create an additional merge commit. Rebase avoids a merge commit by replaying the commits from <code>feature_branch</code> on top of <code>main</code>. After a rebase, the history will look like this:</p>

<div>
	<pre><code>A - B - C         main
         \
          D - E   feature_branch
</code></pre>

  </button>
</div>
</details>


```bash
    git switch -c update_dune COMMITHASH
```
<p>
    Replace <code>COMMITHASH</code> with the hash of the
    <code>D</code> commit, which you can get with a
    <a
    href="https://git-scm.com/docs/git-log"
    target="_blank"
    rel="noopener nofollow"
    >git log
    </a>
    command.
</p>

<ol start="2">
    <li>
        <input type="checkbox" id="checkbox-1" /><label
            for="checkbox-1"
            >Verify with <code>git log --oneline -n 1</code> that you are on the
            new branch and that <code>D</code> is the last commit.</label
        >
    </li>
</ol>
