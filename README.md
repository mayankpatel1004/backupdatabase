1)	Mysqldump through command prompt : 

	go to bin directory example :
	cd D:\wamp64\bin\mysql\mysql5.7.19\bin
	Select your database (slimframework3) name and apply Following command: 
	mysqldump -u root -p slimframework3 > D:/Download/slimframework3.sql
	D:/Download/ = Directory path to save dump.

2) BACKUP ALL DATABASE (STRUCTURE AND DATA)

	mysqldump -u username -p –all-databases > D:\Download\alldb.sql
	OR
	mysqldump -u username -p -A > D:\Download\alldb.sql


3) BACKUP ALL DATABASE (STRUCTURE ONLY)

	mysqldump -u username -p –all-databases –no-data > D:\Download\allstructure.sql
	OR
	mysqldump -u username -p -A -d > D:\Download\allstructure.sql


4) To back up from a remote server, add the -h argument to declare the host address, for example:

	mysqldump -u root -h 182.168.0.120 -p -A > D:\Download\alldb.sql
