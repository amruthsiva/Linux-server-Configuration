# Linux-server-Configuration

## About
  This is the Udacity project 6 about Linux-server-Configuration.

## Details of the server
Server IP Address 13.232.78.196

Hosted site Url [http://13.232.78.196.xip.io/](http://13.232.78.196.xip.io/)

## Grader Password
unix

## Grader Key

-----BEGIN RSA PRIVATE KEY-----
MIIEpQIBAAKCAQEAzil/QJv3Fte5bwFNRtcAjoBRXo2eE7zYyA+nJiEB/+xkL/XK
EjWV3eMA9p53pFyQSVL//X3KYRB50W2sUmY+Y2hZv9iesLRpSD+9qFZuti1Kjlvk
ZYG1pH4Uaz4s+0awX01yb3WBndvxSFoFcvvl4TX5RchDiJhWITdJtwkyT+w3Bjqs
QKb+DlUJFrc9zNwQS74cThmD1M4IHRuFRRq0MwVi14gDQ6uRB6uesP2kD473YpfR
vL6RFZpPj7l5KF56StM6Fai1dXMaBIhwDGmB+4syWsc5tECsfNVPaVeWi1mt3GBy
niIfRcRuxI11CvMlqchZYFdZJQKrtemXKkAl/QIDAQABAoIBAQC8Gji1JpjoCqRy
l+l+PSWQ35tefjBBKglRYJbNv0gnzfQLnmNlAedfsINsgWIAYUR04noXO/KvZW0A
nOShuhAqe0eIN4lzCOkWtrHBKjuRlPl1snpN829cSn0u7Gf2TKUYD33eHITLF6aq
sRhPtW4lci2icfrMYtITNHLZwlZZfDT1+mJ9hFO4KILri6lKq07DhIJYfJg03hEE
HGIKqqwnr7vX7BHOgV9TJ1QaxA1oR9qpruKk6EfiLkbxmSo+jtzOq2WDvllbj+Gu
ZhqCBBF5bGF0whjato74Nm3eZQMDZs11AB/6hGjFemvRkcH1EGUHRjJ0rb3GKb9v
GHEhb7OBAoGBAPXrZpxThDpCEAVObkzN9DeBFFGDF64bi3+tg7MDgojzynpqfMLi
dLq5gIBHJzLBuV3OkczV+FEmrD9sEA4gjJZcLXzp7t/7rpvEnEW4uANWS2G12Hvx
MgqRX6R/OF7aQOnktLUjfgxiZ7Hy3NSV5Jecfy8fgJjC0h/3XA+zQTdZAoGBANac
5QxQOblZg8OqoXTUjaB0rqou1SuQgpJtckqdMUDdmgEjfi+0yYVntRjj5zloLyaG
0EejV1h2dtWxTSH6GR2RayvIvp/H65V+23+6boEa6A4D1zRqtl0VPQbWYbl/JxzL
jOTfQ96DG1Cfw57NGlyzCnsE4j+5gvGrB+/ZobNFAoGBALUWAbpNmYnYyblOltRB
uHsCtvaLBO31ZJTBLcCtbfrxIoFgVryfSvuQy7oqKwgqNRiJmz1ttmvzgVU2euAc
Qcoa2HgqPvd6eopDjhudOQtkCSBLar1hz8qOYBJeiCD4sGJLQnI8T35JHDiiMNDu
C6VE3TbTCLv0ggx99rGs+vIJAoGAKdIrJEoh5YeXELMYgW7GJoV2X/1+Vt3zQ9uG
ERouteg5EY28EknVl2SNOst2jI5L2eMdhUhERh3XrG6/jCZzbHqg+shEtVg9BUXS
OkK3M/ttSwXekv1UijEQUlvGcWJg2dCkpRkI3byIvx5S/YgUYgoVucFK4YYiCTv9
8PRk+U0CgYEAvz7B/2Ns5o8hQhHCE9TnUvJClYkFlel3HzmsuRMZJPFV7iwqMLSf
XWFBA7GlYD4DEq5No3kBsLlX+c+3CIw8UwJ85ikqokG29MwAiYMTsSoL/NVmzLew
WNBRR/bAd6jc1FPZujWgPIvFf107XEX3aSlOu19Kvk3fFP0jzWOVLLU=

-----END RSA PRIVATE KEY-----

## Pub key

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDOKX9Am/cW17lvAU1G1wCOgFFejZ4TvNjID6cmIQH/7GQv9coSNZXd4wD2nnekXJBJUv/9fcphEHnRbaxSZj5jaFm/2J6wtGlIP72oVm62LUqOW+RlgbWkfhRrPiz7RrBfTXJvdYGd2/FIWgVy++XhNflFyEOImFYhN0m3CTJP7DcGOqxApv4OVQkWtz3M3BBLvhxOGYPUzggdG4VFGrQzBWLXiANDq5EHq56w/aQPjvdil9G8vpEVmk+PuXkoXnpK0zoVqLV1cxoEiHAMaYH7izJaxzm0QKx81U9pV5aLWa3cYHKeIh9FxG7EjXUK8yWpyFlgV1klAqu16ZcqQCX9 sathish@Sathish


## To connect as grader:
  
  save private key provided in your local machine and run the following command
  ```
  ssh -i path/to/privatekey -p 2200 grader@13.232.78.196
    
  ```
## Linux Server Configuring

### Update all packages
```
sudo apt-get update
sudo apt-get upgrade
```

### Create grader User:
  ```
  sudo adduser grader
  ```
  New user will be added
  ```
  sudo nano /etc/sudoers
  ```
  Append the following line using below the Root user 
  ```
  grader  ALL=(ALL:ALL) ALL
  ```
  Sudo permission to grader will be granted
  
  ### Creating a ssh key pair for grader
  
   On your local machine in terminal/command prompt
   ```
   ssh-keygen
   ```
   This will generate public and private ssh keys which is saved to .ssh folder
   
   Then in your virtual machine change to newly created user
   ```
   sudo su - grader
   ```
   Create a new directory .ssh and new file authorized_keys in that directory
   ```
   mkdir .ssh
   sudo nano .ssh/authorized_keys
   ```
   Copy the public key with .pub extension to authorized_keys and save the file
   ```
   chmod 700 .ssh
   chmod 644 .ssh/authorized_keys
   ```
   - 700 will give read write and execute permission to user.
   - 644 prevent other user from writting in to file.
   Restart ssh server
   ```
   sudo service ssh restart
   ```
   
   Now log in to grader with private key generated 
   ```
   ssh -i .ssh/id_rsa grader@ipaddress 
   ```
  ### Changing the ssh port to 2200
   ```
   sudo nano /etc/ssh/sshd_config
   ```
   Change port 22 to port 2200
    
   Restart the ssh server
   
   ```
   service ssh restart
   ```
   
   >Note: Before Logging using ssh add custom TCP port 2200 under lightsaail firewall in networking tab in lightsail instance console  
   
   Now Login using command like this
   ```
   ssh -i .ssh/id_rsa -p 2200 grader@ipaddress
   ```
   
  ### Disabling ssh login as root
  `sudo nano /etc/ssh/sshd_config`
  
  make change `PermitRootLogin no`
  
  ### Configurating  Ufw firewall
  ```
  sudo ufw allow 2200/tcp
  sudo ufw allow 80/tcp
  sudo ufw allow 123/udp
  sudo ufw enable
  ```
  This will allow all required ports and enables the ufw
  
  Next 
  ```
  sudo ufw status
  ```
  It will display all allowed ports
  
  ### Change time Zone
  `sudo dpkg-reconfigure tzdata`
  
  select none from list and then select utc.
  
  ### Install Apache2 
  In terminal 
  ```sudo apt-get install apache2```
  
  Now mod_wsgi
  
  ```sudo apt-get install python-setuptools libapache2-mod-wsgi```
  
  Enable mod_wsgi
  
  ```sudo a2enmod wsgi ```
  #### Setup your flask application to work with apache2
   Creating a flask app
   
   In /var/www directory create a new folder
   `sudo mkdir FlaskApp`
   
   Install git 
   
   `sudo apt-get install git`
   
   move to the FlaskApp `cd FlaskApp`
   
   In that direcory clone your github repository
   
   `sudo git clone https://github.com/username/catalog.git`
   
   Rename your repository to FlaskApp
   
   Then rename your project file to `__init__.py`
   
   >Error : While accesssing the client_secret.json file 
   ```
   PROJECT_ROOT = os.path.realpath(os.path.dirname(__file__))
   json_url = os.path.join(PROJECT_ROOT, 'client_secrets.json')
   CLIENT_ID = json.load(open(json_url))['web']['client_id']
   ```
   Use json_url instead client_secret.json in script
   
   Reffered from [stack overflow](https://stackoverflow.com/questions/44742566/wsgi-cant-find-file-in-same-directory-in-app)
   
  #### Install and configuring postgresql for project
   Install Postgres `sudo apt-get install postgresql`
   
   login to postgres `sudo su - postgres`
   
   postgres shell `psql`
   
   create user `CREATE USER catalog WITH PASSWORD 'password';`
   
   permit user to createdb `ALTER USER catalog CREATEDB;`
   
   Create a db name  catalog with user catalog `CREATE DATABASE catalog WITH OWNER catalog;`
   
   connect to db `\c catalog`
   
   revoke all permission to public `REVOKE ALL ON SCHEMA public FROM public;`
   
   Give schema permission to user catalog `GRANT ALL ON SCHEMA public TO catalog;`
   
   exit from db  `\q`
   exit from postgres `exit`
   
   Change the database connection in both db_setup.py and __init__.py as `engine =       create_engine('postgresql://catalog:password@localhost/catalog')`
   
   Now you are ready with your applicatiom
  ### Configure and Enable a New Virtual Host
   `sudo nano /etc/apache2/sites-available/FlaskApp.conf`
   
   In this add the following code
   ```
   <VirtualHost *:80>
		ServerName mywebsite.com
		ServerAdmin admin@mywebsite.com
		WSGIScriptAlias / /var/www/FlaskApp/flaskapp.wsgi
		<Directory /var/www/FlaskApp/FlaskApp/>
			Order allow,deny
			Allow from all
		</Directory>
		Alias /static /var/www/FlaskApp/FlaskApp/static
		<Directory /var/www/FlaskApp/FlaskApp/static/>
			Order allow,deny
			Allow from all
		</Directory>
		ErrorLog ${APACHE_LOG_DIR}/error.log
		LogLevel warn
		CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
   ```
   Enable the virtual host 
   `sudo a2ensite FlaskApp`
   
   Disabling the default apache2 page
   `sudo a2dissite 000-default.conf`
   
  ### Create the .wsgi File
    ```
    cd /var/www/FlaskApp
    sudo nano flaskapp.wsgi 
    ```
   Add the following code
   
   ```
   #!/usr/bin/python
    import sys
    import logging
    logging.basicConfig(stream=sys.stderr)
    sys.path.insert(0,"/var/www/FlaskApp/")

    from FlaskApp import app as application
    application.secret_key = 'Add your secret key'
   ```
   save and exit
   
   Deploying flask app with apache2 is referred from [Digital ocean](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
  
   ### Installing require modules
   Install modules
   To Create virtual environment: sudo virtualenv venv
   To activate virtual environment: source venv/bin/activate
   ` pip install flask sqlalchemy psycopg2 requests oauth2client`

   To deactivate virtual environment: deactivate
   
   ### Setting up your Google Oauth2
   Login to your [developer console](https://console.developers.google.com) and select your project and edit OAuth details as following
   
   Javascript origin
   `http://ip.xip.io`
   
   redirect URI
   
   `http://ip.xip.io\callback`
   
   `http://ip.xip.io\gconnect`
   
   `http://ip.xip.io\login`
   
   [xip.io](xip.io) is a free DNS which will be the same as using IP address
   
   ### Last Step
   Restart your apache2 server
   
   `sudo service apache2 restart`
   
   ### References used
        https://www.digitalocean.com
        and some done github projects to get an idea 
