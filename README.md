MySQL Backup:
Backup data for the wordpress MySQL database is located in the "mysqlbackup" directory.
To restore the database, follow these steps:
1. Access the database via the frontend using the following command: "mysql -u cis527 -p -h 10.108.0.3" then enter the password for the cis527 user.
2. Create a new database to dump your backup data into by using the following command "CREATE DATABASE wordpress;"
3. Exit mySQL using the following command "exit".
4. Copy the "mysqlbackup" directory into the home folder.
5. Complete dumps for each database in the directory using the following example command as a template "mysql -u cis527 -p -h 10.108.0.3 wordpress < wordpress_backup.sql"
(Additonal information can be located in the following guide: "https://www.digitalocean.com/community/tutorials/how-to-backup-mysql-databases-on-an-ubuntu-vps")

Apache2 and Wordpress backup:
The restore for Apache2 and Wordpress are located in the "apache_backup.tar.gz" file.
1. To restore the file, first copy this file into the home directory.
2. Then run the following command in the terminal from the home directory "tar -xzvf apache_backup.tar.gz -C /etc/apache2/".
(Additonal information can be located in the following guide: "https://www.howtogeek.com/248780/how-to-compress-and-extract-files-using-the-tar-command-on-linux/")
