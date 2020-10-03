# WSL Setup

* [cURL](https://curl.haxx.se/)
* [Make](https://www.gnu.org/software/make/manual/make.html)
* [Node.js v12 / npm](https://nodejs.org/)
    * [npm-check-updates](https://www.npmjs.com/package/npm-check-updates)
* [yarn](https://yarnpkg.com/)
* [Vue CLI](https://cli.vuejs.org/)
* [Heroku CLI](https://heroku.com/)
* [Vercel CLI](https://vercel.com/)
* [Asciinema](https://asciinema.org/)
* [PHP7.4](https://www.php.net/)
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


**cURL**
```bash
sudo apt-get install curl
```

**Make**
```bash
sudo apt-get install make
```

**Node.js v12 / npm**
```bash
sudo apt-get update
sudo apt-get upgrade -y
sudo curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install nodejs -y
sudo npm install -g npm-check-updates
sudo chown -R $USER:$(id -gn $USER) /home/bvlad/.config
```

**yarn**
```bash
sudo apt-get update
sudo apt-get install yarn -y
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
sudo npm i -g varcel
```

**Asciinema**
```bash
sudo apt-add-repository ppa:zanchey/asciinema
sudo apt-get update
sudo apt-get install asciinema
```
**PHP7.4**
```bash
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt update
sudo apt install php7.4-fpm php7.4-common php7.4-mysql php7.4-gmp php7.4-curl php7.4-intl php7.4-mbstring php7.4-xmlrpc php7.4-gd php7.4-xml php7.4-cli php7.4-zip php7.4-sqlite3
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
