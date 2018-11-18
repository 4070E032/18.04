# 18.04
sudo wget https://www.apachefriends.org/xampp-files/7.2.11/xampp-linux-x64-7.2.11-0-installer.run
sduo chmod 777 xampp-linux-x64-7.2.11-0-installer.run
sudo ./xampp-linux-x64-7.2.11-0-installer.run



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
