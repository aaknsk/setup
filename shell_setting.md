## .bashrc

```
# "-F":ディレクトリに"/"を表示 / "-G"でディレクトリを色表示
alias ls='ls -FG'
alias ll='ls -alFG'
alias lh='ls -hlFG'
```

## .bash_profile

### ■git setting

```sh
export PATH=$PATH:$HOME/.nodebrew/current/bin
if [ -f ~/.bashrc ] ; then
. ~/.bashrc
fi

source /git/git-prompt.sh
source /git/git-completion.bash
GIT_PS1_SHOWDIRTYSTATE=true
export PS1='\[\033[32m\]\u@\h\[\033[00m\]:\[\033[34m\]\w\[\033[31m\]$(__git_ps1)\[\033[00m\]\n\$ '
```

### ■reference
- [【macOS】プロンプトにgitのブランチ名を出す方法](https://qiita.com/tamorieeeen/items/a5ce73fc4c0f8e825557)