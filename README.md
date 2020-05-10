# WSL Setup

* [cURL](https://curl.haxx.se/)
* [Node.js v12 / npm](https://nodejs.org/)
* [yarn](https://yarnpkg.com/)
* [Vue CLI](https://cli.vuejs.org/)
* [Heroku CLI](https://heroku.com/)
* [Vercel CLI](https://vercel.com/)
* [Asciinema](https://asciinema.org/)
* [PHP7.3](https://www.php.net/)
* [Composer](https://getcomposer.org/)
* [WP CLI](https://wp-cli.org/)

## Install
**Ubuntu 18.04**
* Open PowerShell as Administrator and run:
```bash
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```
* Restart your computer when prompted.
* [Install Ubuntu 18.04](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)


**Node.js v12 / npm**
```bash
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install curl
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get -y install nodejs
sudo chown -R $USER:$(id -gn $USER) /home/bvlad/.config
```

**yarn**
```bash
sudo apt-get update
sudo apt-get install yarn
```

**Vue CLI**
```bash
sudo npm i -g @vue/cli
```

**Heroku CLI**
```bash
sudo curl https://cli-assets.heroku.com/install.sh | sh
```

**Varcel CLI**
```bash
sudo npm i -g now
```

**Asciinema**
```bash
sudo apt-add-repository ppa:zanchey/asciinema
sudo apt-get update
sudo apt-get install asciinema
```
**PHP7.3**
```bash
sudo apt install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt update && sudo apt install php7.3 php7.3-common php7.3-mysql php7.3-xml php7.3-xmlrpc php7.3-curl php7.3-gd php7.3-imagick php7.3-cli php7.3-dev php7.3-imap php7.3-mbstring php7.3-opcache php7.3-soap php7.3-zip php7.3-intl -y
```

**Composer**
```bash
sudo curl -s https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
```

**WP CLI**
```bash
curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
chmod +x wp-cli.phar
sudo mv wp-cli.phar /usr/local/bin/wp
```

**Create SSH key**
```bash
ssh-keygen -t rsa -C "your_email@example.com"
```