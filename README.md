# Setup of development environment on new ubuntu instalation

## 0- install build essentials:
`sudo apt install build-essential`


## 1-download node lts through nvm:

https://github.com/nvm-sh/nvm#installation-and-update

## 2-download yarn:

https://yarnpkg.com/en/docs/install#debian-stable

## 3-download git:

### 3.1 - open terminal: Ctrl + Alt + T

### 3.2 - update registry(require super user privileges): sudo apt update

### 3.3 - install git: sudo apt-get install git

## 4-install vscode:

### 4.1 - get the vscode .deb option: https://code.visualstudio.com/download

### 4.2 - double click on the downloaded file of previous step, then click install

### 4.3 - install the following extensions:

#### 4.3.1 - Vetur(for Vuejs development)

#### 4.3.2 - Eslint(for javascript code lint)

#### 4.3.3 - Prettier(for javascript code format)

#### 4.3.4 - vscodeicons(for good file iconography)

#### 4.3.5 - Bracket Pair Colorizer(for better nesting visualization)

#### 4.3.6 - Darktooth Theme(for nice color theme)

#### 4.3.7 - ES7 React/Redux/GraphQl...(for React development)

## 5-install sublime:

Search for Sublime on Ubuntu Software, then click install

### 6-install docker:

#### 6.1 - open terminal: Ctrl + Alt + T

#### 6.2 - update registry(require super user privileges): sudo apt update

#### 6.3 - istall docker: sudo apt install docker.io

#### 6.4 - set docker to run on OS startup:

##### 6.4.1 - sudo systemctl start docker

##### 6.4.2 - sudo systemctl enable docker

#### 6.5 - check docker version: docker --version

#### 6.6 - elevate docker user privileges(may need OS restart): sudo usermod -a -G docker \$USER

### 7-install rust(may be outdated, if so, check the current rust book for instalation guide):

https://doc.rust-lang.org/1.5.0/book/installing-rust.html

#### 7.1 - install gcc(some rust libs may require for dependencies compilation)


## 8 - install vim:
### 8.1 - update registry(require super user privileges): sudo apt update
### 8.2 - get vim-gnome through apt-get: sudo apt-get install vim-gnome
### 8.3 - create vim configuration file .vimrc on /home/$USER: cd /home/$USER && touch .vimrc
### 8.4 - install vim-plug: https://github.com/junegunn/vim-plug
### 8.5 - get vim the vim configuration template on: https://gist.github.com/Nickrosendo/12432136abbddc3157da0c7a2f3257fe
### 8.6 - paste the content of the template on your .vimrc and save the file
### 8.7 - install plugins: `:PlugInstall`
### 8.8 - copy minimalist colors folder to .vim/: `cp -r /home/$USER/.vim/plugged/minimalist/colors /home/$USER/.vim/`

## 9 - install zsh: 
### 9.1 - https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH
### 9.2 - install ohmyzsh: https://github.com/ohmyzsh/ohmyzsh
### 9.3 - set zsh theme: ZSH_THEME='clean'
### 9.4 - set vim as default editor: `export EDITOR=$(which vim)`

## 10 - install tmux: 
### 10.1 - `sudo apt-get install tmux`
### 10.2 - install tmux theme: https://github.com/gpakosz/.tmux
