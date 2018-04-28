# Basic Commands

To initialize a git repository (to command git to track files), we use command:

`git init`

Git stores all tracking information in `.git` directory. If you remove .git directory, git won't track files.

- To add all the changes to this directory use command:

`git add .`

To add single file to staging area:

`git add <filename>`

- To commit these additions, command:

`git commit -m "Message for the commit"`

For git, commit messages need to be meaningful. It should be short summary (< 50 characters), optionally followed by blank line and more description. Keep each line less than 72 characters. Write commit messages in present tense, not pass tense.

#35345 - Fixes bug in admin logout

- To check the logs of commit messges:

`git log`

It has commit ID, author and date when committed.

`git log -n <number>` will return only number of git log

`git log --since=2016-06-17` shows everything since given date.

`git log --until=2017-05-21` will find commits upto given date

`git log --author="Name of Author"` will give commits by author.

`git log --grep="Init"` will find any regular expression commit messages with "Init".

**Git uses three-tree architecture.**

Repository (on remote repo)
Staging index
working (on local machine)

Git creates hash for each commit and that is also called commit id. Git maintains HEAD pointer to point to the HEAD of the references. It goes to the current branch of the repository.
