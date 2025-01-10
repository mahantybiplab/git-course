### When to Rebase

git rebase and git merge are different tools.

An advantage of merge is that it preserves the true history of the project. It shows when branches were merged and where. One disadvantage is that it can create a lot of merge commits, which can make the history harder to read and understand.

A linear history is generally easier to read, understand, and work with. Some teams enforce the usage of one or the other on their <code>main</code> branch, but generally speaking, you'll be able to do whatever you want with your own branches.

### Warning

You should never rebase a public branch (like <code>main</code>) onto anything else. Other developers have it checked out, and if you change its history, you'll cause a lot of problems for them.

However, with your own branch, you can rebase onto other branches (including a public branch like <code>main</code>) as much as you want.


<details>
    <summary> Rebasing <code>Feature</code> Branch onto <code>Main</code> Branch or Rebasing <code>Main</code> Branch onto <code>Feature</code> Branch
    which one is considered good?</summary>

    In this context, "onto" refers to changing the base of one branch to align with another branch's latest commit history. It essentially means placing one branch's commits on top of another branch's commits.

    It's a bad manners to rebase a public branch onto your own personal branch

    It's generally okay to merge changes into your own private branch, or to rebase your branch onto a public branch

</details>