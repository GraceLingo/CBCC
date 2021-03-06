# coreui-laravel
CCBC Web App based on CoreUI-Laravel

CoreUI-laravel is simple adaptation to Laravel the most beautiful free Bootstrap 4 admin template created by Lukasz Holeczek

![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_charts.png)

Prerequisites
- XAMPP (https://www.apachefriends.org/xampp-files/7.2.6/xampp-win32-7.2.6-0-VC15-installer.exe)
- Composer (https://getcomposer.org/Composer-Setup.exe)
- Git and Git Bash (https://git-scm.com/download/win)

### Installation
- To Start Installation 
```bash
Open XAMPP and start Apache and MySQL
```

- To clone repository
```bash
git clone git@github.com:bluedeveloper1/cbc.git
cd cbc
composer install
cp .env.example .env
php artisan key:generate
```

- To change name in browser
```bash
Open notepad (Run as administrator). File > Open.
Go to C:\Windows\System32\drivers\etc\hosts
Put in the last line
	127.0.0.1 localhost
	127.0.0.1 cbc.me
Save.
Go to C:\xampp\apache\conf\extra\httpd-vhosts.conf and add the ff in the last line.
	<VirtualHost *:80>
		DocumentRoot "C:/xampp/htdocs"
		ServerName localhost
	</VirtualHost>

	<VirtualHost *:80>
		DocumentRoot "C:/xampp/htdocs/cbc/public"
		ServerName cbc.me
		<Directory "C:/xampp/htdocs/cbc/public">
			Order allow,deny
			Allow from all
		</Directory>
	</VirtualHost>
Save.
```

- To create table in database
```bash
Go to http://localhost/phpmyadmin/
Create database (Click Databases)named cbc
```

Go to GIT

```bash
	php artisan migrate
```

- To start the app
```bash
Open browser (preferably Chrome).
Go to cbc.me
Go to Register
Register
You will be directed to main page.
```



##### That's all. Enjoy.

### Change log
##### v 1.0.6a
##### v 1.0.6
- Update to CoreUI 1.0.6
- In gulpfile.js prepared scripts to import libraries and app files to /public directory

## Screenshots

![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_charts.png)
![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_cards.png)
![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_charts.png)
![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_switches.png)
![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_tabs.png)
![alt text](https://raw.githubusercontent.com/taboritis/coreui-laravel/master/sample_widgets.png)
