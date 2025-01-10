```bash
    git config --add --global user.name "ThePrimeagen"
    git config --add --global user.email "the.primeagen@aol.com"

    git config --add --local user.name "ThePrimeagen"
    git config --add --local user.email "the.primeagen@aol.com"

    git config --list --local

    git config --get <key> # key = <section>.<keyname>
    git config --unset <key>

    cat .git/config

    git config --unset-all example.key 
    # The --unset-all flag is useful if you ever really want to purge all instances of a key from your configuration. Conversely, the --unset flag only works with a single instance of a key.

    git config --remove-section section # section = webflyx
```

<details>
    <summary style="font-size:18px">Locations</summary>
    <p>
      There are several locations where Git can be configured. From more general
      to more specific, they are:
    </p>
    <ul>
      <li>
        <strong>system</strong>: <code>/etc/gitconfig</code>, a file that
        configures Git for all users on the system
      </li>
      <li>
        <strong>global</strong>: <code>~/.gitconfig</code>, a file that
        configures Git for all projects of a user
      </li>
      <li>
        <strong>local</strong>: <code>.git/config</code>, a file that configures
        Git for a specific project
      </li>
      <li>
        <strong>worktree</strong>: <code>.git/config.worktree</code>, a file
        that configures Git for part of a project
      </li>
    </ul>
</details>

```bash
    $HOME = ~/
```