## log in to my sql as root

//without root password

sudo mysql -u root 

//with root password

sudo mysql -u root -p

## create DB, user, grant access
'''sql
create databse mytestdb;

create user myuser identified by "mypass";

use mytestdb;

GRANT ALL PRIVILEGES ON mytestdb.* to myuser;

flush privileges;
'''
## LOG IN USING THE NEW USER

mysql -u myuser -p
 enter password:(enter "mypass" here)
 mysql ->
 