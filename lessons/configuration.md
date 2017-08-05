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

`git config --global user.name "Your Username"
git config --global user.email "youremail@email.com"`

You can list git configuration using `--list` flag.

`git config --list`

OR

`git config user.email` and `git config user.name`

All these configurations are stored at `~/.gitconfig`. To open that file follow these commands.

`cd ~
cat .gitconfig`

- To configure text editor with git:

`git config --global core.editor "gedit -wl1"`

- To configure colors for git:

`git config --global color.ui true`
