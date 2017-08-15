Implementing Oracle Database Server on AWS
(A)DESIGN A PLAN
-Decide on the physical location of the EC2 server.  Having a server in close proximity of end users will prevent latency 
 issues.
*AWS offers the following zones:  US East (N. Virginia), US East (Ohio), US West (N. California), US West (Oregon), Canada (Central), 
EU (Ireland), EU (Frankfurt), EU (London), Asia Pacific (Singapore), Asia Pacific (Sydney), Asia Pacific (Seoul), Asia Pacific (Tokyo), 
Asia Pacific (Mumbai), South America (Sao Paulo)*.
-Contingent with the scope of the project, AWS offers low to high-end servers available via the launch instance wizard. 
 For my dev project I selected a general purpose server on a windows platform.  
(B)LAUNCH THE INSTANCE WIZARD
(C)STORAGE OPTIONS
-Ideally storage options should be decidined when planning.  However, since I found out 30 gb would not be enough, I provisioned 
 more storage via Volumes on the EC2 dashboard.
(D)FIREWALL
 -A static IP is required for firewall configuration. Use the elastic IP option on the AWS managment console to assign a static/permenate 
 IP (AWS console).  This will prevent you from having to enter a different IP to connect to your server every 
 time.   
 -You will need to setup the ip, port, and protocol you plan on using to connect to your server through security groups before being able 
 to do so. 
 
 Implementing Oracle 11g Database Server
 -Connect to your server via SSH or RDP, download the correct version of the oracle database that matches your platform.
 -Be sure that you have enough space partioned on your hard drive for the installation.
 -Once this is done run the installation wizard (if on linux go to OTN for instructions on the installation process).
 -Configure your database and create an administrative password.
 -Once this is done download and install Oracle SQL developer to allow you to administer your new database.
 
 Implementing Microsoft SQL Database Server
 -Connect to your server via SSH or RDP, download the correct version of Microsoft SQL Server.
 -Be sure that you have enough space partioned on your hard drive for the installation.
 -Run the installation wizard.
 -Configure your database and create an administrative password.
 -Microsoft SQL Server comes with SQL Server Managment Studio, use this to edit and administer your database.
