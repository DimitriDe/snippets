# Ubuntu 15.04 post installation

Update repositories and packages

    sudo apt-get update
    sudo apt-get upgrade

Install common programs

    sudo apt-get install audacious hexchat gimp inkscape meld filezilla gedit-plugins
    sudo apt-get install unity-tweak-tool virtualbox gftp dillo
    sudo apt-get install homebank chromiumbsu chromium gufw gparted scribus

Install console programs

    sudo apt-get install htop links irssi cowsay nmap mpg123 traceroute p7zip-full
    sudo apt-get install finger subversion git mesa-utils rar unrar dos2unix

Servers

    sudo apt-get install ssh apache2 mysql-server libapache2-mod-php5 php5-mysql php5-gd php5-mcrypt
    sudo php5enmod mcrypt
    sudo a2enmod rewrite
    sudo a2enmod userdir
    
    edit /etc/apache2/envvars if you want apache to run with a different user
    don't forget to chown -R /var/log/apache2 /var/lock/apache2 /var/run/apache2 /var/www with the correct user and group
    
Install Java :

    #download oracle java for your platform
    tar -xvzf jre-8uXX-linux-x64.tar.gz
    sudo mkdir /usr/local/java
    sudo mv jre1.8.0_XX/ /usr/local/java/
    sudo update-alternatives --install "/usr/bin/java" "java" "/usr/local/java/jre1.8.0_77/bin/java" 1
    java -version
    #java version "1.8.0_XX"
    #Java(TM) SE Runtime Environment (build 1.8.0_XX-yyy)
    #Java HotSpot(TM) 64-Bit Server VM (build aa.bb-yyy, mixed mode)

Flat os theme :

    sudo add-apt-repository ppa:noobslab/themes
    sudo add-apt-repository ppa:noobslab/icons
    sudo apt-get update
    sudo apt-get install flatabulous-theme
    sudo apt-get install ultra-flat-icons
