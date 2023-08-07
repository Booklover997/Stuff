[[Config File]] for [[zsh]] on [[Linux]] using [[Antigen]]  as a [[bundler]] and [[power10k]] as a theme
```

Enable Powerlevel10k instant prompt. Should stay close to the top of ~/.zshrc.

# Initialization code that may require console input (password prompts, [y/n]

# confirmations, etc.) must go above this block; everything else may go below.

if [[ -r "${XDG_CACHE_HOME:-$HOME/.cache}/p10k-instant-prompt-${(%):-%n}.zsh" ]]; then

  source "${XDG_CACHE_HOME:-$HOME/.cache}/p10k-instant-prompt-${(%):-%n}.zsh"

fi

  

# Created by newuser for 5.8.1

  

source ~/antigen.zsh

alias cat=ccat

# Load the oh-my-zsh's library.

antigen use oh-my-zsh

  

# Bundles from the default repo (robbyrussell's oh-my-zsh).

antigen bundle git

antigen bundle heroku

antigen bundle pip

antigen bundle lein

antigen bundle docker

antigen bundle command-not-found

antigen bundle autojump

# Syntax highlighting bundle.

antigen bundle zsh-users/zsh-syntax-highlighting

antigen bundle zsh-users/zsh-autosuggestions

antigen bundle zsh-users/zsh-completions

antigen bundle hcgraf/zsh-sudo

antigen bundle ael-code/zsh-colored-man-pages

# Load the theme.

antigen theme romkatv/powerlevel10k

  

# Tell Antigen that you're done.

antigen apply

  

# To customize prompt, run `p10k configure` or edit ~/.p10k.zsh.

[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh

```