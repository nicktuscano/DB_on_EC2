Implementing a Database Server on AWS EC2

(A)DESIGN AN ARCHITECTURE PLAN
-Decide on the physical host location (zone) of the EC2 server.  Having a server in close proximity of end users will reduce network latency 
 issues.
*AWS offers the following zones:  US East (N. Virginia), US East (Ohio), US West (N. California), US West (Oregon), etc.*
-Contingent on the scope of the project, AWS offers low to high-end servers available via the launch instance wizard. For new AWS 
customers, a free tier is offered; however modest fees are still assessed for usage above the free tier limits. 
-For my dev project I selected a general purpose EC2 server on a windows platform.  

(B)LAUNCH THE INSTANCE WIZARD

(C)STORAGE OPTIONS
-Ideally storage options should be decided during planning.  However, since I found out the starter 30 gb would not be enough, I 
provisioned additional storage via Volumes on the EC2 dashboard after the server was already in production.

(D)FIREWALL
 -A static IP is required for firewall configuration. Use the elastic IP option on the AWS managment console to assign a static/permanent 
 IP.  This will prevent you from having to enter a different IP to connect to your server every time.  That is if you let the IP be 
 dynamically assigned.   
 -You will need to setup the ip, port, and protocol you plan on using to connect to your server through security groups before being able 
 to do so (remote server administration). 
 
 Implementing Oracle 11g Database Server (*)
 -Connect to your EC2 server via SSH (Linux) or RDP (Windows); download the version of the oracle database that matches your 
  server OS platform.
 -Be sure that you have enough space partioned on your hard drive for the installation.
 -Once this is done run the installation wizard (if on linux go to Oracle Technology Network for instructions on the installation 
 process).
 -Configure your database and create an administrative password.
 -Once this is done download and install Oracle SQL developer client to allow you to administer your new database from a remote client.
 
 Implementing Microsoft SQL Database Server (*)
 -Connect to your EC2 server via SSH (Linux) or RDP (Windows), download the correct version of Microsoft SQL Server.
 -Be sure that you have enough space partioned on your hard drive for the installation.
 -Run the installation wizard.
 -Configure your database and create an administrative password.
 -Microsoft SQL Server comes with SQL Server Managment Studio, use this to edit and administer your database.
 
 (*) For dev purposes Oracle offers Oracle database Server Express and SQL Developer for free. Microsoft offers SQL Server Express 
 and SQL Server Managment Studio for client admin which are also both free.
 
 Some Images
 
AWS EC2 Instance: ![](https://github.com/nicktuscano/DB_on_EC2/blob/master/1a_Instance.png)
AWS EC2 Elastic IP: ![](https://github.com/nicktuscano/DB_on_EC2/blob/master/1b_Instance%2BElasticIP.png)
AWS EC2 Security Groups: ![](https://github.com/nicktuscano/DB_on_EC2/blob/master/1c_SecurityGroups.png)

