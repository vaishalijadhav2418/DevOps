Absolutely! Here are **40 common Git and GitHub interview questions** complete with concise answers—without including real-time scenarios:

---

### 🔹 **Basic Git Questions (1–10)**

1. **What is Git?**
   Git is a distributed version control system used to track changes in source code during software development.

2. **How is Git different from centralized version control systems?**
   Each developer has a local repository, enabling offline commits, full history, and better branching compared to centralized systems like SVN.

3. **What is a Git repository?**
   A directory containing `.git` metadata, commit history, branches, tags, and objects.

4. **Explain the difference between `git clone`, `git fetch`, and `git pull`.**

   * `clone`: creates a local copy of a remote repo
   * `fetch`: downloads remote changes without merging
   * `pull`: fetches and merges remote changes into the current branch

5. **What is the staging area in Git?**
   Also called "index"; it's where changes are prepared before committing.

6. **How do you undo a staged change?**
   Use: `git reset HEAD <file>` to unstage a file.

7. **How do you revert a committed change?**
   Use: `git revert <commit>` to create a new commit reversing the changes.

8. **What is the difference between `git reset` and `git revert`?**

   * `reset`: moves branch pointer (can rewrite history)
   * `revert`: safely adds a new commit, preserving history

9. **Explain the difference between `git merge` and `git rebase`.**

   * `merge`: combines branches with a merge commit
   * `rebase`: applies commits from one branch onto another, rewriting history

10. **What is a Git branch? How do you create one?**
    A branch is a movable pointer to a commit. Use `git branch <name>` or `git checkout -b <name>` to create and switch to it.

---

### 🔹 **Branching & Merging (11–20)**

11. **Explain fast-forward vs three-way merge.**

    * Fast-forward: no divergent history, simply moves the branch pointer
    * Three-way merge: creates a new commit to merge divergent histories

12. **What is `git cherry-pick` used for?**
    To selectively apply a specific commit from one branch to another.

13. **How do you resolve merge conflicts?**
    Manually edit conflicting files, stage them, and then run `git commit` to finalize the merge.

14. **What are Git tags, and how are they used?**
    Tags are references to specific commits, usually for marking releases (e.g., `v1.0`).

15. **Explain difference between annotated and lightweight tags.**

    * Annotated: stored as full objects with metadata
    * Lightweight: just a simple pointer, no extra metadata

16. **Can you delete a branch in Git? How?**
    Yes:

    * Local: `git branch -d <branch>`
    * Remote: `git push origin --delete <branch>`

17. **What is `git stash` and when to use it?**
    Temporarily saves uncommitted changes so you can work on another task.

18. **How do you apply a stash?**
    Use `git stash apply` to reapply changes or `git stash pop` to apply and drop it.

19. **What is a reflog?**
    A log of branch and HEAD movements, useful for recovering lost commits.

20. **How do you recover an accidentally deleted branch?**
    Use reflog to find the commit: `git reflog`, then create a branch: `git branch <name> <commit>`.

---

### 🔹 **Working with Remotes & Collaboration (21–30)**

21. **How do you add a remote repository?**
    Use: `git remote add origin <url>`.

22. **How do you push a new branch to remote?**
    Use: `git push -u origin <branch-name>`.

23. **How do you force push, and when should you use it?**
    Use: `git push --force`. Use cautiously when rewriting history and only if collaborators are aware.

24. **What is a pull request?**
    A request to merge changes from one branch to another, usually reviewed by peers before merging.

25. **How do you resolve conflicts in GitHub pull requests?**
    Pull the branch locally, resolve conflicts, commit, and push—GitHub updates the PR automatically.

26. **What are GitHub forks and how are they used?**
    A personal copy of a repository enabling independent changes that can later be submitted via pull requests.

27. **What is GitHub Flow?**
    A lightweight workflow: create branches per feature, open PRs, review, merge to main, deploy.

28. **What is GitHub Actions?**
    A CI/CD platform integrated into GitHub to automate workflows like testing and deployment.

29. **What are submodules in Git?**
    Pointers to other repositories embedded in a parent repo. Useful for external dependencies.

30. **How do you update a submodule?**
    Use `git submodule update --remote` to fetch and update tracked commits.

---

### 🔹 **Advanced Git (31–40)**

31. **What is Git rebase interactive mode?**
    `git rebase -i` allows squashing, reordering, and editing commits before pushing.

32. **When should you use interactive rebase?**
    To clean up commit history—combine minor fixes, edit messages, reorder commits.

33. **What is `git bisect`?**
    A binary search tool to find which commit introduced a bug by testing revisions.

34. **What is a shallow clone and why use it?**
    Use `git clone --depth=1` to clone without full history, making it faster and smaller.

35. **Explain reflog expiration and cleanup.**
    Reflog entries expire after defaults (90 days), cleaned by `git gc`.

36. **How do you squash multiple commits into one?**
    Use interactive rebase: `git rebase -i HEAD~N`, then mark commits as `squash`.

37. **How do you rewrite commit history across multiple commits?**
    Use `git rebase -i`, change commit messages, authors, or remove commits.

38. **What is `git gc` for?**
    Garbage collection—cleans up unreachable objects, compresses files for performance.

39. **How do you remove tracked files from Git but keep them locally?**
    Use `.gitignore`, then `git rm --cached <file>` to stop tracking.

40. **Explain the concept of “detached HEAD.”**
    Occurs when HEAD points to a commit (not a branch). New commits won’t belong to any branch. To save changes, create a new branch.

