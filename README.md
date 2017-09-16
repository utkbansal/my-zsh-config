# My ZSH Configuration

![Screenshot](https://raw.githubusercontent.com/utkbansal/my-zsh-config/master/screenshot/Screenshot.png)

### Credits
This uses **iTerm2** & **oh-my-zsh** and is heavily inspired by the [agnoster](https://github.com/agnoster/agnoster-zsh-theme) theme!

## Setup Instructions

### Download [iTerm2](https://www.iterm2.com/)
and move it to your Appplications Folder

### Install zsh and zsh-syntax-highlighting
Run this command in your terminal
```bash
brew install zsh zsh-syntax-highlighting
```

### Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
Run this command in your terminal
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Install zsh Plugins
1. Open `zsh` shell and run the following commands
  ```
  git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
  ```
2. Update the `~/.zshrc` file to update the list of plugins
  ```
  plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
  ```

### Install the zsh-theme
1. Copy the file `zsh.zsh-theme` to `~/.oh-my-zsh/themes`
1. Update the `~/.zshrc` file to update the current theme
  ```
  ZSH_THEME="lalit"
  ```
  
### Update iTerm Prefrences

#### Install the Inconsolata for Powerline on your Mac
1. The file is under `/fonts/Inconsolata for Powerline.otf`
1. iTerm > Preferences > Profile > Text > Change Font and select `Inconsolata for Powerline`

#### Install the Color Theme
1. Double click the `zsh.itermcolors`
1. Select the Color Scheme iTerm > Preferences > Profile > Colors > Color Presets --> Select `zsh`


**Note**
You may have to restart the shell to see the changes being reflected
