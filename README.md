sudo apt update
sudo apt upgrade -y
sudo apt install i3 i3status dmenu -y
sudo apt install git
sudo apt install apt-transport-https curl
sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg arch=amd64] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list
sudo apt update
sudo apt install brave-browser
sudo apt remove firefox
sudo apt autoremove
wget -O ~/discord.deb "https://discordapp.com/api/download?platform=linux&format=deb"
sudo dpkg -i discord.deb 
sudo apt --fix-broken install
sudo dpkg -i discord.deb 
sudo snap install zoom-client
sudo apt install volumeicon-alsa
sudo apt install -y git
sudo dpkg -i synergy_1.14.2-stable.c6918b74_ubuntu21_amd64.deb 
sudo apt --fix-broken  install
sudo dpkg -i synergy_1.14.2-stable.c6918b74_ubuntu21_amd64.deb 
sudo apt install tree
sudo apt install openssh-server
curl -sLS https://get.arkade.dev | sudo sh
ark get kubectl
sudo mv /home/dashaun/.arkade/bin/kubectl /usr/local/bin/
ark get k3sup
sudo mv /home/dashaun/.arkade/bin/k3sup /usr/local/bin/
ark get kubens
sudo mv /home/dashaun/.arkade/bin/kubens /usr/local/bin/
ark get kubectx
sudo mv /home/dashaun/.arkade/bin/kubectx /usr/local/bin/
sudo apt install clusterssh

##Git
git config --global init.defaultBranch main
git config --global user.email "dashaun@dashaun.com"
git config --global user.name "DaShaun"

