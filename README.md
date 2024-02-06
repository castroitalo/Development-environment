# Development Envorinment

<p>This is my personal development environment.</p>

## Basic [Ubuntu](https://ubuntu.com/) configuration:

- On **Settings**:
  - **Network**: Add the Google DNS (8.8.8.8).
    - **Power**: Select the Performance option.
    - **Display**: Enable Factional Scaling.
    - **Keyboard**: Setup keyboard shortcuts.
- Install NVIDIA drivers on **Additional drivers**.
- Install [Google Chrome](https://www.google.com/intl/pt-BR/chrome/):
  - Download **.deb** file and install it with:
    - `sudo dpkg -i <deb_file>`
- Enable minimize on dock click:
  - `gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'`
- Install codecs and Microsoft fonts:
  - `sudo apt install ubuntu-restricted-extras`
- Install GNOME extensions:
  - `sudo apt install chrome-gnome-shell`
    - Extensions that I use:
      - [Vitals](https://extensions.gnome.org/extension/1460/vitals/)
      - [Audio Output Switcher](https://extensions.gnome.org/extension/751/audio-output-switcher/)

## Setting up programs

### My dotfiles [here](https://github.com/gnulll/dotfiles)

<em>This is all my pieces of software, not just for development.</em>

- [KeePassXC](https://keepassxc.org/) - Password manager.
  - Install libfuse:
    - `sudo apt install libfuse2`
  - Download KeePassXC AppImage file.
  - To be able to execute KeePassXC give it permission to be executable.
  - I put all my appimages files in a folder called **AppImages** inside my **Documents** folder.
- Login into Google and online accounts.
- My web tools:
  - [devicons.io](https://devdocs.io/)
  - [Regex101](https://regex101.com/)
  - [gitignore.io](https://www.toptal.com/developers/gitignore/)
  - [choosealicense](https://choosealicense.com/)
  - [4devs](https://www.4devs.com.br/)
  - [JSON Formatter](https://jsonformatter.org/)
  - [UUID Generator](https://www.uuidgenerator.net/version4)
  - [Replt](https://replit.com/)
  - [Packagist](https://packagist.org/)
  - [Notion](https://www.notion.so/)
  - [Trello](https://trello.com/)
  - [Excalidraw](https://excalidraw.com/)
  - [StackEdit](https://stackedit.io/)
  - [ChatGPT](https://chat.openai.com/)
  - [GitHub](https://github.com/)
- [Git](https://git-scm.com/) - Versioning tool.
  - `sudo apt install git -y`
  - `git config --global user.name <username>`
  - `git config --global user.email <user_email>`
  - `git config --global core.editor nvim`
  - `ssh-keygen -t rsa -b 4096 -C <user_email>`
- [curl](https://curl.se/) - CLI for transferring data.
  - `sudo apt install curl -y`
- [tmux](https://github.com/tmux/tmux/wiki) - Terminal multiplexer.
  - `sudo apt install tmux -y`
- [htop](https://github.com/htop-dev/htop) - Process viewer.
  - `sudo apt install htop -y`
- [neofetch](https://github.com/dylanaraps/neofetch) - A CLI sysinfo tool.
  - `sudo apt install neofetch -y`
- [net-tools](https://github.com/ecki/net-tools) - Basic network tools.
  - `sudo apt install net-tools -y`
- [Docker](https://www.docker.com/) - Developing platform
  - Oficial documentation for Debian installation [here](https://docs.docker.com/engine/install/ubuntu/)
- [ZSH](https://www.zsh.org/) - Shell.
  - `sudo apt install zsh -y`
  - `chsh -s $(which zsh)`
  - Reboot.
  - [OhMyZsh](https://ohmyz.sh/) - ZSH framework.
    - `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
    - Install [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) plugin:
      - `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
- [PHPStorm](https://www.jetbrains.com/pt-br/phpstorm/) - IDE
  - Download the **tar.gz** file.
  - Extract the **tar.gz** file inside **/opt** folder:
    - `sudo tar -xzf PhpStorm-*.tar.gz -C /opt`
  - Esecute the **phpstorm.sh** file.
  - Create a desktop entry clicking on gear button on the **Welcome** screen.
- [Node.js](https://nodejs.org/en) - JavaScript runtime
  - Install Node.js via NVM [here](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating)
  - List Node versions with `nvm ls-remote`
  - Install a Node version with `nvm install <version>`
  - Change the current Node version with `nvm use node-<version>`
- [qBittorrent](https://www.qbittorrent.org/download) - Torrent client.
  - `sudo apt install qbittorrent -y`
- [Spotify](https://www.spotify.com/br-pt/download/linux/) - Music Player.
  - `sudo snap install spotify`
- [OBS-Studio](https://obsproject.com/pt-br/download) - Open Broadcast Software.
  - `sudo snap install obs-studio`
- [VLC](https://www.videolan.org/vlc/index.pt_BR.html) - Media player.
  - `sudo apt install vlc -y`
- [GIMP](https://www.gimp.org/) - Image editor
  - `sudo apt install gimp -y`

Easy Peasy Lemon Squeezy 👌
