AWS EC2 Server Implementation & Managment
    -Implemented a Ubuntu server on AWS EC2
      -Ran into errors when attempting to install Oracle 11g database
    -Implemented a Windowss server on AWS EC2
      -Successfully installed & administered Oracle 11g database & Windows database
     
    ORACLE DB ADMINISTRATION
    -Created a new user
      -gave permissions to create a table
      -received an error when I attempted to create a table under this user
    -Troubleshooting
      -created a new user
      -granted more concise permissions
      -still received the same error
      -entered this command under system
        (ALTER USER <username> QUOTA UNLIMITED ON <tablespace>)
      -this solved the problem
    -Created data spread sheet
    -Imported data from the excel spread sheet to an SQL table
    -Created a view
      -Created criteria within a View 
