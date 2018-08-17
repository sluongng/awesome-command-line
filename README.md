# awesome-command-line
An opinionated guide to an ideal command line environment

## Linux

- Terminator

## MacOS

- Iterm
- Brew: https://brew.sh/

## Shell

- ZSH:

  https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH

  Linux
  ```shell
  # Linux
  sudo apt-get install zsh
  
  # MacOS
  brew install zsh zsh-completions
  
  chsh -s $(which zsh)
  ```
  
- Oh-my-zsh:

  https://github.com/robbyrussell/oh-my-zsh#basic-installation
  
  ```shell
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  ```
  
- Essential Oh-my-ZSH plugins:
  ```
  plugins=(
    docker
    docker-compose
    git
    sudo
    zsh-autosuggestions
    mvn
    node
    kubectl
    zsh-better-npm-completion
    spring
    golang
    zsh-autosuggestions
  )
  ```
  
## Binaries

- FZF: Fuzzy search over commandline history and file path (built with Golang)
- RipGrep: Faster `grep` (built with Rust)
- FD: Faster `find` (built with Rust)
- Exa: Improved `ls` (built with Rust)
- Bat: Improved `cat` (built with Rust)
