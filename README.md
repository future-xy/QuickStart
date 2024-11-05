# Qinitial

Quick Initailization Package

## Quick Start

```bash
echo `sudo apt update
sudo apt install zsh wget curl vim -y
sudo apt install rsync git build-essential -y

(type -p wget >/dev/null || (sudo apt update && sudo apt-get install wget -y)) &&
	sudo mkdir -p -m 755 /etc/apt/keyrings &&
	wget -qO- https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo tee /etc/apt/keyrings/githubcli-archive-keyring.gpg >/dev/null &&
	sudo chmod go+r /etc/apt/keyrings/githubcli-archive-keyring.gpg &&
	echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | sudo tee /etc/apt/sources.list.d/github-cli.list >/dev/null &&
	sudo apt update &&
	sudo apt install gh -y

sudo apt install fd-find silversearcher-ag htop -y
sudo apt install bat -y` > sudo_install.sh
sudo bash sudo_install.sh
git clone https://github.com/future-xy/QuickStart.git
cd QuickStart
bash install.sh
bash config.sh
```

## Package Components

### sudo_install

1. Improve shell: `zsh`
2. Network: `curl`, `wget`
3. Git: `gh`, `git`
4. Basic compile: `build-essential`
5. Pyenv/Anaconda depedencies
6. CLI tools: `fd`(a better find), `ag`(a better grep), `bat`(a better cat)

### install

1. Python virtual environment management: `pyenv`
2. Vimrc: from [github/vimrc](https://github.com/amix/vimrc)
3. Nvim and Nvim config: provided by [@Chivier](https://github.com/Chivier)
4. zsh config: .zinit and zshrc
5. tmux config: from [github/tmuxrc](https://github.com/rxrc/tmuxrc)
6. lazygit: a cli git tool

### install Anaconda

```bash
pyenv install anaconda3-2024.02-1
```

### install docker and docker-compose

```bash
sudo bash install_docker.sh
```


### TODO

Update module management to TINA

