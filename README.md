# Oh my zsh.

## Install with curl
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Enabling Plugins (zsh-autosuggestions & zsh-syntax-highlighting)
 - Download zsh-autosuggestions by

 `
 git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
 `

 - Download zsh-syntax-highlighting by

 `
 git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
 `

 - `nano ~/.zshrc` find `plugins=(git)`

 - Append `zsh-autosuggestions & zsh-syntax-highlighting` to  `plugins()` like this

 `plugins=(git zsh-autosuggestions zsh-syntax-highlighting)`

 - Reopen terminal

 ## zsh-completions

   Clone the repository inside your oh-my-zsh repo:

  git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:-${ZSH:-~/.oh-my-zsh}/custom}/plugins/zsh-completions

  Add it to FPATH in your .zshrc by adding the following line before source "$ZSH/oh-my-zsh.sh":

  fpath+=${ZSH_CUSTOM:-${ZSH:-~/.oh-my-zsh}/custom}/plugins/zsh-completions/src

 ## zsh-256colors

    cd $ZSH_CUSTOM/plugin

    git clone https://github.com/chrissicool/zsh-256color

