## Enable Snap && Icons

```
sudo mv /etc/apt/preferences.d/nosnap.pref ~/Documents/nosnap.backup
sudo ln -s /var/lib/snapd/desktop/applications/ /usr/share/applications/snap
```

## Docker/Compose / Snap / Git / Make / TG / Sublime / PHPStorm

```
sudo add-apt-repository ppa:git-core/ppa -y sudo apt update
sudo apt install -y git make docker-compose snapd
```
```
sudo snap install telegram-desktop
sudo snap install phpstorm --classic
sudo snap install sublime-text --classic
```

## Permissions

```
sudo usermod -aG sudo ${USER}
sudo usermod -aG www-data ${USER}
sudo usermod -aG docker ${USER}
```

`sudo visudo` > `volkv ALL=(ALL) NOPASSWD:ALL`


## SSH keys

```
sudo chmod 700 ~/.ssh
chmod 600 ~/.ssh/*
```
