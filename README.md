
# awesome-command-line

An opinionated guide to an ideal command line environment

## Linux

- Terminator
- Linuxbrew: http://linuxbrew.sh/

## MacOS

- Iterm
- Brew: https://brew.sh/

## Shell

<details>
<summary>ZSH</summary>

  https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH

  Linux

  ```shell

  # Linux
  sudo apt-get install zsh
  
  # MacOS
  brew install zsh zsh-completions
  
  chsh -s $(which zsh)

  ```
</details>
  
<details>
<summary>Oh-my-zsh</summary>

  https://github.com/robbyrussell/oh-my-zsh#basic-installation
  
  ```shell
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  ```
</details>

<details>
<summary>Essential Oh-my-ZSH plugins</summary>

  ```text

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

  ## TODO: split this into language specific section

  ```
  
  - zsh-autosuggestions:

    https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md

    ```shell
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    ```
</details>

## Binaries / CLI toolings

<details>
<summary>
<b>JQ:</b> JSON prettifier, powerful data extraction tool (built with C)
</summary>

  https://stedolan.github.io/jq/download/

  ```shell
  sudo apt install jq
  brew install jq
  ```
</details>

<details>
<summary>
<b>Pup:</b> HTML data extraction (built with Golang)
</summary>

  https://github.com/ericchiang/pup#install

  ```shell
  go get github.com/ericchiang/pup

  brew install https://raw.githubusercontent.com/EricChiang/pup/master/pup.rb
  ```
</details>

<details>
<summary>
<b>XMLStarlet:</b> XML data extraction (written in C)
</summary>

  (**do not recommend** because its not very intuitive)

  ```shell
  sudo apt search xmlstarlet
  ```
</details>

<details>
<summary>
<b>FZF:</b> Fuzzy search over commandline history and file path (built with Golang)
</summary>
  
  https://github.com/junegunn/fzf#installation

  ```shell
  brew install fzf

  # To install useful key bindings and fuzzy completion:
  $(brew --prefix)/opt/fzf/install
  ```
</details>

<details>
<summary>
<b>RipGrep:</b> Faster `grep` (built with Rust)
</summary>

  https://github.com/BurntSushi/ripgrep#installation

  ```shell
  brew install ripgrep
  sudo apt install ripgrep
  ```
</details>

<details>
<summary>
<b>FD:</b> Faster `find` (built with Rust)
</summary>

  https://github.com/sharkdp/fd#installation

  ```shell
  brew install fd

  # Linux
  # https://github.com/sharkdp/fd/releases
  ```

  - Note: This can be use in combination with FZF to search and navigate through directory tree even faster
</details>

<details>
<summary>
<b>Exa / LSD:</b> Improved `ls` (built with Rust)
</summary>
  Both Exa and LSD are rust implementation of gnu `ls` command
  The different is that Exa is **NOT** in active development thus I would recommend using LSD instead

  https://github.com/Peltoche/lsd#installation
  
  ```shell
  brew install lsd

  cargo install lsd
  
  alias ls=lsd
  ```
  
  https://github.com/ogham/exa#installation

  ```shell
  brew install exa
  
  cargo install exa
  ```
</details>

<details>
<summary>
<b>Bat:</b> Improved `cat` (built with Rust)
</summary>

  https://github.com/sharkdp/bat#installation

  ```shell
  brew install bat
  cargo install bat
  ```
</details>


<details>
<summary>
<b>FastMod:</b> Improved `sed` (built with Rust)
</summary>
  Facebook awesome code refactoring tool using Rust regex (same lib as FD and Ripgrep)
  
  See Also: https://github.com/facebook/codemod, https://github.com/facebookarchive/pfff/

  https://github.com/facebookincubator/fastmod

  ```shell
  cargo install fastmod
  ```
</details>

<details>
<summary>
<b>Mycli:</b> Commandline `mysql` with autocorrect (built with Python)
</summary>

  https://github.com/dbcli/mycli#quick-start

  ```shell
  brew install mycli

  sudo apt install mycli
  ```

  - Postgres: https://github.com/dbcli/pgcli#quick-start

  - MSSQL / SQL Server: https://github.com/dbcli/mssql-cli#mssql-cli
</details>

## Additional Notes

- More information on usages, tips and tricks [HERE](https://github.com/sluongng/awesome-command-line/issues?utf8=%E2%9C%93&q=is%3Aissue+sort%3Aupdated-desc+)
