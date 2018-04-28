# Undo changes

If by mistake, we delete some part of the program and then we want it back, we can use:

`git checkout <filename>`

It brings the file back and changes are restored.

**Unstage**

`git reset HEAD <filename>`

**Undo commits**

It is possible to change the last commit.

`git commit --amend -m "Commit message"`

We can revert the commit using
`git revert <sha of commit>`
