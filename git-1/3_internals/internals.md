<p>
    You may have noticed that even though we (you and I) both have the
    <strong>same content</strong> in our repositories, we have
    <strong>different commit hashes</strong>. While commit hashes
    <em>are</em> derived from their content changes, there's
    <a
    href="https://git-scm.com/book/en/v2/Git-Internals-Git-Objects#_git_commit_objects"
    target="_blank"
    rel="noopener nofollow"
    >also some other stuff</a
    >
    that affects the end hash. For example:
</p>
<ul>
    <li>The commit message</li>
    <li>The author's name and email</li>
    <li>The date and time</li>
    <li>Parent (previous) commit hashes</li>
</ul>

<style>
  .details {
    color: rgb(15, 188, 188);
    font-size: 24px;
  }
</style>

<details>
    <summary class="details">
    It's Just Files All the Way Down
    </summary>
    <p>All the data in a Git repository is stored directly in the (hidden) <code>.git</code> directory. That includes all the commits, branches, tags, and other objects we'll learn about later.</p>
    <p>Git is made up of <a href="https://git-scm.com/book/en/v2/Git-Internals-Git-Objects" target="_blank" rel="noopener nofollow">objects</a> that are stored in the <code>.git/objects</code> directory. A commit is just a type of object.</p>
</details>

<h3>Cat File</h3>

```bash
    git cat-file -p <hash>
    Use the cat-file command to view the contents of your commit
```

<ul>
    <li><code>tree</code>: git's way of storing a directory</li>
    <li><code>blob</code>: git's way of storing a file</li>
</ul>

<details>
    <summary class="details">Storing Data</summary>
    <div style="padding:20px;">
        Git stores an entire snapshot of files on a per-commit level.
        <details>
            <summary style="color:rgb(15, 188, 188); font-size:18px">Optimization</summary>
            <p>While it's true that Git stores entire snapshots, it <em>does</em> have some performance optimizations so that your <code>.git</code> directory doesn't get too unbearably large.</p>
            <ul>
                <li>Git <a href="https://git-scm.com/book/en/v2/Git-Internals-Packfiles" target="_blank" rel="noopener nofollow">compresses and packs</a> files to store them more efficiently.</li>
                <li>Git deduplicates files that are the same across different commits. If a file doesn't change between commits, Git will only store it once.</li>
            </ul>
        </details>
    </div>
</details>
