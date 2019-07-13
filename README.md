# zsh-config
My .zshrc config for backup *macOS*


0. install homebrew and iterm2

`xcode-select —-install`

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

`brew cask install iterm2`


1. install zsh

`brew install zsh zsh-completions`

`sudo port install zsh zsh-completions`


2. install oh-my-zsh

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

`upgrade_oh_my_zsh`


3. install powerlevel10k zsh theme

`git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k`

(Set in your ~/.zshrc.)

> ZSH_THEME=powerlevel10k/powerlevel10k 


4. install bright lights iterm2 theme

`https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/schemes/Bright%20Lights.itermcolors`

(Set iterm2 shell to /bash/zsh)

(Set theme to above)


5. install zsh autosuggestions

`git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions`

(Add the following to your .zshrc:)

> source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh


6. install zsh syntax highlighting

`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git`

`echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc`


7. install source code powerline regular font

`git clone https://github.com/powerline/fonts.git`

`cd fonts`

`./install.sh`
