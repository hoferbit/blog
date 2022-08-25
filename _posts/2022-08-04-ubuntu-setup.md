---

layout: post
title: Ubuntu Setup
categories: Tool
description: Tool
keywords: macOS,Tool

---

# zsh oh-my-zsh
```sh
# install zsh
echo $SHELL
cat /etc/shells
apt update && apt install zsh -y
chsh -s /bin/zsh
reboot

# install oh-my-zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# config oh-my-zsh
vim ~/.zshrc # ZSH_THEME="bira"
source ~/.zshrc

git clone https://github.com/zsh-users/zsh-autosuggestions.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
vim ~/.zshrc # plugins=(git zsh-syntax-highlighting zsh-autosuggestions)
alias gitpull="git pull"
alias gp="git add . && git commit -m 'build' && git push
source ~/.zshrc 
```

apt-get install net-tools  