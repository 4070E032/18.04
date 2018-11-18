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

#下載DVWA檔

sudo wget https://github.com/ethicalhack3r/DVWA/archive/master.zip

#給予DVWA檔執行權限


sudo chmod 777 master.zip

#解壓縮DVWA檔


sudo unzip master.zip

#將解壓縮的檔案移動至/opt/lampp/htdocs


sudo mv DVWA-master /opt/lampp/htdocs


'''

'''

#進入至/opt/lampp/htdocs

cd /opt/lampp/htdocs/DVWA-master/config

#更改config.inc.php.dist的檔案名稱


sudo mv config.inc.php.dist config.inc.php

#下載編譯程式


sudo vim config.inc.php


$_DVWA[ 'db_user' ] = 'root';

$_DVWA[ 'db_password' ] = '';

$_DVWA[ 'recaptcha_public_key' ] = '6LfQNCYTAAAAALx0oAwtLHJlzNHXTKLl2UZjQjw-';

$_DVWA[ 'recaptcha_private_key' ] = '6LfQNCYTAAAAAHnvqCzw2lG95FD-RfomKHWf7Zob';

$_DVWA[ 'default_security_level' ] = 'low';


#修改php.ini內容  


sudo vim /opt/lampp/etc/php.ini

#allow_url_include = On 
位於(46%)的位子


#重啟XAMPP

sudo /opt/lampp/lampp restart

#開啟DVWA
在瀏覽器輸入127.0.0.2/DVWA-master 進入頁面

#登入後點選
SQL Injection

#進入之後輸入 1’or’1’=‘1 

會看到其他的帳號以及密碼

#end
