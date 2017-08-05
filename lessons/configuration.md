# Basic Configuration

- System level configuration: default configuration for git all users on the same system. It is inside etc/gitconfig

- User level configuration: It is inside ~/.gitconfig
- Project level configuration: <projectname>/.git/config

You can modify configuration using:

System level:
`git config --system`

User level:
`git config --global`

Project level:
`git config`

For example,

`git config --global user.name "Your Username"'

'git config --global user.email "youremail@email.com"`

You can list git configuration using `--list` flag.

`git config --list`

OR

`git config user.email` and `git config user.name`

All these configurations are stored at `~/.gitconfig`. To open that file follow these commands.

`cd ~
cat .gitconfig`

- To configure text editor with git:

`git config --global core.editor "gedit"`

- To configure colors for git:

`git config --global color.ui true`

## Git autocompletion feature:

For Windows, it already includes auto-completion.
For Unix systems,

`cd ~`

`curl -OL https://github.com/git/git/raw/master/contrib/completion/git-completion.bash`

`mv ~/git-completion.bash ~/.git-completion.bash`

`nano .bash_profile`

Add the following script in `.bash_profile` file.

```bash
if [ -f ~/.git-completion.bash ]; then
  source ~/.git-completion.bash
fi
```

This gives you auto-completion feature in Git.

## How to get help in Git

Use `git help` to get help.
To get help on any command, use:

```git
git help <command>
```

For example,

```git
git help log
```

to move to the next page in command line use 'f', for backward 'b' or you can scroll using 'UP' and 'DOWN' arrow keys.
