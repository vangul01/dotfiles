# dotfiles

For MacBook Pro with the M1 chip 😎

## Terminal

### Jsons for iTerm oh-my-zsh terminal configurations

[Andromeda.json](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/41890c50-d176-4a61-8074-7c000d640e2a/Andromeda.json)

### Color Profiles

[ciapre.itermcolors](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8183176e-f4e6-4e72-b26c-3aa6b3571970/ciapre.itermcolors)

### Installs and Updates

1. Install iTerm2
    1. I just did this online by downloading it
2. Install oh my zsh!

    ```bash
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    ```

3. Update .zshrc file

    ```bash
    # If you come from bash you might have to change your $PATH.
    # export PATH=$HOME/bin:/usr/local/bin:$PATH

    # Path to your oh-my-zsh installation.
    export ZSH="/Users/valerieangulo/.oh-my-zsh"

    # Set name of the theme to load --- if set to "random", it will
    # load a random theme each time oh-my-zsh is loaded, in which case,
    # to know which specific one was loaded, run: echo $RANDOM_THEME
    # See https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
    ZSH_THEME="robbyrussell"

    # Uncomment the following line to use case-sensitive completion.
    # CASE_SENSITIVE="true"

    # Uncomment the following line to use hyphen-insensitive completion.
    # Case-sensitive completion must be off. _ and - will be interchangeable.
    HYPHEN_INSENSITIVE="true"

    # Uncomment the following line if pasting URLs and other text is messed up.
    # DISABLE_MAGIC_FUNCTIONS="true"

    # Uncomment the following line to disable auto-setting terminal title.
    # DISABLE_AUTO_TITLE="true"

    # Uncomment the following line to enable command auto-correction.
    # ENABLE_CORRECTION="true"

    # Uncomment the following line to display red dots whilst waiting for completion.
    # Caution: this setting can cause issues with multiline prompts (zsh 5.7.1 and newer seem to work)
    # See https://github.com/ohmyzsh/ohmyzsh/issues/5765
    # COMPLETION_WAITING_DOTS="true"

    # Uncomment the following line if you want to disable marking untracked files
    # under VCS as dirty. This makes repository status check for large repositories
    # much, much faster.
    # DISABLE_UNTRACKED_FILES_DIRTY="true"

    # Uncomment the following line if you want to change the command execution time
    # stamp shown in the history command output.
    # You can set one of the optional three formats:
    # "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
    # or set a custom format using the strftime function format specifications,
    # see 'man strftime' for details.
    # HIST_STAMPS="mm/dd/yyyy"

    # Would you like to use another custom folder than $ZSH/custom?
    # ZSH_CUSTOM=/path/to/new-custom-folder

    # Which plugins would you like to load?
    # Standard plugins can be found in $ZSH/plugins/
    # Custom plugins may be added to $ZSH_CUSTOM/plugins/
    # Example format: plugins=(rails git textmate ruby lighthouse)
    # Add wisely, as too many plugins slow down shell startup.
    plugins=(git)

    source $ZSH/oh-my-zsh.sh

    # Set personal aliases, overriding those provided by oh-my-zsh libs,
    # plugins, and themes. Aliases can be placed here, though oh-my-zsh
    # users are encouraged to define aliases within the ZSH_CUSTOM folder.
    # For a full list of active aliases, run `alias`.
    #
    # Example aliases
    # alias zshconfig="mate ~/.zshrc"
    # alias ohmyzsh="mate ~/.oh-my-zsh"
    alias zshconfig="vi ~/.zshrc"
    alias refresh="source ~/.zshrc"

    # python
    alias ipy="ipython3"
    alias py="python2"
    alias py3="python3"

    # for git
    alias gitcls="git rm -r --cached"
    alias gi="git init"
    alias ga="git add"
    alias gc="git commit"
    alias gd="git diff"
    alias gr="git reset"
    alias gm="git merge"
    alias gpu="git push"
    alias gpl="git pull"
    alias gs="git status"
    alias gch="git checkout"
    alias gb="git branch"
    alias gcl="git clone"
    alias gst="git stash"
    alias gsp="git stash pop"
    alias sos="fsck --cache --no-reflogs --lost-found --dangling HEAD"

    # prompt header
    # PS1='%n@%m %~$ '

    # direnv
    # eval "$(direnv hook zsh)"

    # fasd
    # eval "$(fasd --init auto)"

    # Go
    export GOPATH=$HOME/go
    export PATH=$PATH:$GOPATH/bin

    # autosuggestions
    # source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh

    # virtualenvwrapper
    # export WORKON_HOME=$HOME/.virtualenvs
    # export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3
    # source /usr/local/bin/virtualenvwrapper.sh

    # The next line updates PATH for the Google Cloud SDK.
    # if [ -f '/Users/valerieangulo/google-cloud-sdk/path.zsh.inc' ]; then . '/Users/valerieangulo/google-cloud-sdk/path.zsh.inc'; fi

    # The next line enables shell command completion for gcloud.
    # if [ -f '/Users/valerieangulo/google-cloud-sdk/completion.zsh.inc' ]; then . '/Users/valerieangulo/google-cloud-sdk/completion.zsh.inc'; fi
    ```

4. Remove "last login"

    [https://osxdaily.com/2010/06/22/remove-the-last-login-message-from-the-terminal/](https://osxdaily.com/2010/06/22/remove-the-last-login-message-from-the-terminal/)

    ```bash
    touch ~/.hushlogin
    ```

5. Change default header of terminal

    [https://aheze.medium.com/how-to-change-the-window-title-in-terminal-zsh-oh-my-zsh-ca41f3a35128#:~:text=Now%2C open terminal preferences by,want for the terminal title](https://aheze.medium.com/how-to-change-the-window-title-in-terminal-zsh-oh-my-zsh-ca41f3a35128#:~:text=Now%2C%20open%20terminal%20preferences%20by,want%20for%20the%20terminal%20title)!

## Python

Make sure the default python version is updated. 

**Reference Articles**

 [https://stackoverflow.com/questions/60453261/how-to-default-python3-8-on-my-mac-using-homebrew](https://stackoverflow.com/questions/60453261/how-to-default-python3-8-on-my-mac-using-homebrew)

## Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

==> Next steps:
- Run these two commands in your terminal to add Homebrew to your PATH:
    echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/valerieangulo/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"
```

**Reference Articles**

- [https://apple.stackexchange.com/questions/410825/apple-silicon-port-all-homebrew-packages-under-usr-local-opt-to-opt-homebrew](https://apple.stackexchange.com/questions/410825/apple-silicon-port-all-homebrew-packages-under-usr-local-opt-to-opt-homebrew)
- [https://blog.smittytone.net/2021/02/07/how-to-migrate-to-native-homebrew-on-an-m1-mac/](https://blog.smittytone.net/2021/02/07/how-to-migrate-to-native-homebrew-on-an-m1-mac/)

## Installs

```bash
brew install virtualenvwrapper
brew install direnv
brew install the_silver_searcher
brew install zsh-autosuggestions
brew install fasd
brew install tig
brew install tree
```

## Git Setup

```bash
git config --global user.email "vaa238@nyu.edu"
git config --global user.name "Valerie Angulo"
```

---

**Shortcut Notes**

clear shortcut control L

delete lines command shift K in vs code
