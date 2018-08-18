# awesome-command-line
An opinionated guide to an ideal command line environment

## Linux

- Terminator
- Linuxbrew: http://linuxbrew.sh/

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
  )
  ```
  
  + zsh-autosuggestions:
    
    https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md

    ```shell
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    ```

## Binaries / CLI toolings

- JQ: JSON prettifier, powerful data extraction tool (built with C)

  https://stedolan.github.io/jq/download/

  ```shell
  sudo apt install jq
  brew install jq
  ```

- Pup: HTML data extraction (built with Golang)

  https://github.com/ericchiang/pup#install

  ```shell
  go get github.com/ericchiang/pup

  brew install https://raw.githubusercontent.com/EricChiang/pup/master/pup.rb
  ```

- XMLStarlet: XML data extraction (written in C)

  (**do not recommend** because its not very intuitive)

  ```shell
  sudo apt search xmlstarlet
  ```

- FZF: Fuzzy search over commandline history and file path (built with Golang)
  
  https://github.com/junegunn/fzf#installation

  ```shell
  brew install fzf

  # To install useful key bindings and fuzzy completion:
  $(brew --prefix)/opt/fzf/install
  ```

- RipGrep: Faster `grep` (built with Rust)

  https://github.com/BurntSushi/ripgrep#installation

  ```shell
  brew install ripgrep
  sudo apt install ripgrep
  ```

- FD: Faster `find` (built with Rust)

  https://github.com/sharkdp/fd#installation

  ```shell
  brew install fd

  # Linux
  # https://github.com/sharkdp/fd/releases
  ```

  + Note: This can be use in combination with FZF to search and navigate through directory tree even faster
- Exa: Improved `ls` (built with Rust)

  https://github.com/ogham/exa#installation

  ```shell
  brew install exa
  cargo install exa
  ```

- Bat: Improved `cat` (built with Rust)

  https://github.com/sharkdp/bat#installation

  ```shell
  brew install bat
  cargo install bat
  ```
