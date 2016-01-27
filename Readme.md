# DOLIBARR ERP & CR

Container with installed Dolibarr and all needed tools.
Database is not included, run a mysql and create a database.

Assuming you have a running mysql container:
```
docker run -d --name doli-test --link mysql:mysql -p 80:80 -e "PHP_TIMEZONE=Europe/Amsterdam" zauberertz/dolibarr:3.8.3
```
The ```PHP_TIMEZONE``` is used to set a proper timezone, default is UTC
