# Ubuntu 15.04 post installation

Update repositories and packages

    sudo apt-get update
    sudo apt-get upgrade

Install common programs

    sudo apt-get install audacious hexchat gimp inkscape meld filezilla gedit-plugins
    sudo apt-get install unity-tweak-tool virtualbox gftp dillo

Install console programs

    sudo apt-get install htop links irssi cowsay nmap mpg123 traceroute p7zip-full
    sudo apt-get install finger subversion git mesa-utils rar unrar dos2unix

Servers

    sudo apt-get install ssh apache2 mysql-server php5-mysql php5-gd php5-mcrypt
    sudo php5enmod mcrypt
    sudo a2enmod rewrite
    sudo a2enmod userdir
    
    edit /etc/apache2/envvars if you want apache to run with a different user
    don't forget to chown -R /var/log/apache2 /var/lock/apache2 /var/run/apache2 /var/www with the correct user and group
