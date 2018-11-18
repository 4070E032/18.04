# UBUNTU18.04
'''

#下載XAMPP安裝檔

sudo wget https://www.apachefriends.org/xampp-files/7.2.11/xampp-linux-x64-7.2.11-0-installer.run

#給予XAMPP安裝檔執行權限

sduo chmod 777 xampp-linux-x64-7.2.11-0-installer.run

#執行XAMPP安裝檔

sudo ./xampp-linux-x64-7.2.11-0-installer.run

'''

'''
sudo wget https://github.com/ethicalhack3r/DVWA/archive/master.zip



sudo chmod 777 master.zip


sudo unzip master.zip



sudo mv DVWA-master /opt/lampp/htdocs


'''

'''
#進入至/opt/lampp/htdocs

cd /opt/lampp/htdocs/DVWA-master/config



sudo mv config.inc.php.dist config.inc.php


sudo vim config.inc.php


$_DVWA[ 'db_user' ] = 'root';
$_DVWA[ 'db_password' ] = '';
$_DVWA[ 'recaptcha_public_key' ] = '6LfQNCYTAAAAALx0oAwtLHJlzNHXTKLl2UZjQjw-';
$_DVWA[ 'recaptcha_private_key' ] = '6LfQNCYTAAAAAHnvqCzw2lG95FD-RfomKHWf7Zob';
$_DVWA[ 'default_security_level' ] = 'low';




sudo vim /opt/lampp/etc/php.ini


sudo /opt/lampp/lampp restart
