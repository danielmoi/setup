# MacOS

## Apps
- Docker
- Postico
- Slack
- Firefox
- Chrome
- 1Password
- VSCode
- Monit
- Fanny
- Sonos

- XCode
- IntelliJ
- Sketch

----
## System Preferences
- Keyboard
  - Key Repeat > Fast
  - Delay Until Repeat > Short
  - Modifier Keys
    - Caps Lock > Escape

---
## SSH
- Set up SSH Key and add to Github
  - https://help.github.com/articles/connecting-to-github-with-ssh/

---
## Dock
Add spaces to dock:
```
# space
defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock

# small space
defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="small-spacer-tile";}'; killall Dock
```

---
## Screenshots
defaults write com.apple.screencapture location ~/screenshots

System Preferences > Language & Region > Time format: 24-hour time


---
## VS Code
- install extensions
  - Beautify
  - EditorConfig
  - Emoji
  - ESLint
  - Flow
  - Gitlens
  - npm intellisense
  - Vim
  - vscode-icons
  - viml

- Enable PressAndHold:
    ```
    To disable the Apple press and hold for VSCode only, do this:

    defaults write com.microsoft.VSCode ApplePressAndHoldEnabled -bool false
    ```

Setup ssh key + Github

---
## iTerm
- Profiles
  - General > Reuse previous session's directory
  - Colors > Color presets > Solarized Dark (makes Vim look nice)
  - Terminal > Scrollback Buffer > Unlimited
  - Keys > Load preset > Natural text editing

---
## Command Line Programs
- homebrew
- zsh
- oh-my-zsh
- neovim
- rg
- kubectl
- fzf
- htop
- redis

----
## Neovim
- Install Neovim
  ```
  brew install neovim
  ```
- Setup config
  ```
  # ~/.config/nvim/init.vim

  set runtimepath^=~/.vim runtimepath+=~/.vim/after
  let &packpath = &runtimepath
  source ~/.vimrc
  ```
