### Pull

Fetching is nice, but most of the time we want the actual file changes from a remote repo, not just the metadata.

```bash
    git pull [<remote>/<branch>]
```
The <code>[...]</code> syntax means that the bracketed remote and branch are optional. If you execute git pull without anything specified it will pull your current branch from the remote repo.

### Pull Requests


<p>On GitHub, a <a href="https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests" target="_blank" >pull request</a> is a way to propose changes, typically to the rest of your team, or to the maintainer of a project you're contributing to.</p>

Pull requests allow team members to see what changes are being proposed and to discuss them before they are merged into the main codebase.

- Push the new branch to GitHub (push it to the remote <code>add_classics</code> branch).
- Navigate to the GitHub repo in your browser
- Click on the "Pull requests" tab near the top
- Click "New pull request".
- Set the base branch to <code>main</code> and the compare branch to <code>add_classics</code>, as we plan to merge <code>add_classics</code> into <code>main</code> later.
- Create the pull request, but don't merge it yet!
