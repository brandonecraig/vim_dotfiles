# Create Symlinks

Symlink `vimrc` to `~/.vimrc` and `vim` to `~/.vim`.

Symlink `tmux.conf` to `~/.tmux.conf`

Open vim and run `:PlugInstall`.

# Change shell bash
`chsh -s /bin/bash`

# Install Homebrew

`/bin/bash -c "$(curl -fsSL
https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`

# Install Tmux

`brew install tmux`

# Git Config

`git config --global user.name "Brandon Craig"`
`git config --global user.email brandon.craig@guildeducation.com`

# Install Node

`brew install node`

# Install Yarn

`brew install yarn`

# Install nvm

`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh |
bash`
`nvm alias default 10.14.1`

# Install rvm
`\curl -sSL https://get.rvm.io | bash -s stable --ruby`

# Improve Command Prompt
```
parse_git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
export PS1="bcraig \[\e[32m\]\w \[\e[91m\]\$(parse_git_branch)\[\e[00m\]$ "
```
