# My Terminal Setup

## Terminal Shell
Install ZSH using [Oh My ZSH](https://ohmyz.sh/)

## Place .zshrc file at required place
```
$ cp .zshrc ~/.zshrc
```

## Place .bash_profile file at required place
```
$ cp .bash_profile ~/.bash_profile
```

## Make sure brew is correctly configured and added to .zprofile
```
$ (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/ankushchavan/.zprofile
$ eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Install Oh My Posh
```
$ brew install jandedobbeleer/oh-my-posh/oh-my-posh
```

## Place the custom terminal theme at required place and make sure it is used in .zshrc
```
$ cp ankushtheme.omp.json ~/ankushtheme.omp.json
```

## Change the prompt
### Find the shell
```
$ oh-my-posh get shell
```

### For ZSH shell
```
$ eval "$(oh-my-posh init zsh)"
$ exec zsh
```

### Note:
If you are using warp then make sure to change the terminal promt from the warp's appearance settings
