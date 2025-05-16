# Git Rebase
## Moves local commits on top of remote commits (linear history)
1. Check status:
    ```bash
    git status
    ```
2. If it's clean (no uncommitted changes) the issue `rebase` command:
    ```bash
    git pull --rebase
    ```
3. Then, issue `push` command:
    ```bash
    git push
    ```

