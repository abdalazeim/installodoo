## install odoo
## Fast-Installationsprogramme odoo 16&17 
## install nodejs & rtlcss

[Odoo-16]https://www.odoo.com/documentation/16.0/de/administration/install/packages.html)
[Odoo-17](https://www.odoo.com/documentation/17.0/administration/install/packages.html)
> Ubuntu 22.04
```
sudo apt update; sudo apt upgrade -y

sudo apt install postgresql -y
sudo systemctl status postgresql
sudo -u postgres psql
\q
sudo apt install python3-psycopg2

sudo apt install wkhtmltopdf -y

sudo pip3 install xlwt
sudo pip3 install num2words
pip3 list |grep xlwt
pip3 list |grep num2words
odoo-16
 wget -q -O - https://nightly.odoo.com/odoo.key | sudo gpg --dearmor -o /usr/share/keyrings/odoo-archive-keyring.gpg
 echo 'deb [signed-by=/usr/share/keyrings/odoo-archive-keyring.gpg] https://nightly.odoo.com/16.0/nightly/deb/ ./' | sudo tee /etc/apt/sources.list.d/odoo.list
 sudo apt-get update && sudo apt-get install odoo
Odoo-17
wget -q -O - https://nightly.odoo.com/odoo.key | sudo gpg --dearmor -o /usr/share/keyrings/odoo-archive-keyring.gpg
echo 'deb [signed-by=/usr/share/keyrings/odoo-archive-keyring.gpg] https://nightly.odoo.com/17.0/nightly/deb/ ./' | sudo tee /etc/apt/sources.list.d/odoo.list

sudo apt update && sudo apt install odoo

sudo ufw allow 5432
sudo ufw allow 8069
sudo ufw status numbered

sudo dpkg -l odoo
sudo systemctl status odoo

http://192.168.100.112:8069/

#SI DA ERRROR:
  sudo systemctl stop odoo
  sudo -u postgres psql
  DROP DATABASE odoo;
  sudo systemctl restart postgresql
  sudo systemctl restart odoo


sudo tail -f /var/log/odoo/odoo-server.log

```
path codigo fuente odoo: /usr/lib/python3/dist-packages/odoo
## install nodejs & rtlcss
sudo apt install nodejs
sudo apt install npm
sudo npm install -g rtlcss


install nodejs & rtlcss
sudo apt install nodejs
sudo apt install npm
sudo npm install -g rtlcss


