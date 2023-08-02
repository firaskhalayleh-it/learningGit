

1. `1`
2. `2`
- `-1` (which means removed)
- `+2` (which means added)
3. `no changes be committed`
4. `3`
5. `they removed 1, and added 3`
6. `empty (no changes be committed)`
7. `changes not staged for commit`
8. The log looks like:

```
Commit fdb1aca34615170a22bc772b2db009cf917c5cba:

Author: git-katas trainer bot <git-katas@example.com>
Date: Wed Aug 2 13:04:07 2023 +0300
Commit Message: "1"

Commit (latest):

Author: firas <fkmkh11@gmail.com>
Date: Wed Aug 2 13:14:37 2023 +0300
Commit Message: "commiting"
```

9. `4`
10. `3`
11. `nothing committed`
12. The `git restore` command is used to restore files in the working directory to their state at a specific commit or branch. It helps to undo changes made to tracked files in the working directory. For example, you can use `git restore` to discard local changes and revert files back to their state in the last commit.
