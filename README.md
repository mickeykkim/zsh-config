# zsh-config
My .zshrc config for backup *macOS*

From-scratch installation guide:

0. install homebrew and iterm2 (optionally install vscode as well if desired)

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

`echo "ZSH_THEME=powerlevel10k/powerlevel10k" >> ${ZDOTDIR:-$HOME}/.zshrc`


4. install zsh autosuggestions

`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

(Run the following or manually edit into .zshrc if other plugins already installed (i.e. git)):

`echo "plugins=(zsh-autosuggestions)" >> ${ZDOTDIR:-$HOME}/.zshrc`


5. install zsh syntax highlighting

`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git`

`echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc`


6. install source code powerline regular font

`git clone https://github.com/powerline/fonts.git`

`cd fonts`

`./install.sh`


7. if using vscode: add the following lines to your vscode config

> "terminal.integrated.shell.osx": "/bin/zsh",

> "terminal.integrated.fontFamily": "'SourceCodePro+Powerline+Awesome Regular'",


8. optional: install bright lights iterm2 theme

> https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/schemes/Bright%20Lights.itermcolors

(Set iterm2 shell to /bash/zsh)

(Set theme to above)


9. optional: install plastic vscode theme

> https://vscodethemes.com/e/will-stone.plastic
