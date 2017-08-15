Implementing Oracle Database Server on AWS
(A)Design a plan
-Decide on the physical location of the EC2 server.  Having a server in close proximity of end users will prevent latency 
 issues.
*AWS offers the following zones:  US East (N. Virginia), US East (Ohio), US West (N. California), US West (Oregon), Canada (Central), 
EU (Ireland), EU (Frankfurt), EU (London), Asia Pacific (Singapore), Asia Pacific (Sydney), Asia Pacific (Seoul), Asia Pacific (Tokyo), 
Asia Pacific (Mumbai), South America (Sao Paulo)*.
-Contingent with the scope of the project, AWS offers low to high-end servers available via the launch instance wizard. 
 For my dev project I selected a general purpose server on a windows platform.  
(B)Launch the instance wizard
(C)Ideally storage options should be decidined when planning.  However, since I found out 30 gb would not be enough, I provisioned 
 more storage via Volumes on the EC2 dashboard.
 
 Implementing SQL Server
 
