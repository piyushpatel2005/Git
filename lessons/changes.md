# Making and managing changes

- `git status` can be used to check the status of the git repository.

To check the difference between two files in the project. You can use

`git diff` to check the changes between current local directory and staging index. The changes with + are additions.

If you want to get the difference between staging index and repository, you can use:

`git diff --staged`

When you delete a file and want to add that change to the staging index, we need to use `git rm` command.

`git rm <filename>`

`git commit -m "<filename> deleted"`

- We can rename a file using `git mv` command.

`git mv <filename1> <filename2>`

This will change filename1 to filename2.

We can see only the difference between two long lines by words by using:

`git diff --color=words`

To add and commit the changes to the repository use:

`git commit -am "commit message"`

This only works for modifications but newly added files are not tracked.
