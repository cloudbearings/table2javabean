table2javabean
==============
-------------
# Overview
This tool is designed to help developer quick produce Java Bean source file
from an existed sql table . It is implemented by dos batch and easy to use and config .
So far, Only mysql is supported .
 
#  Testing Enviroment
- Windows7 through
- Others   NT
 
 
# Usage
Run this script from CLI and enter requirement parameters when
prompted . if  no error occurs, a Java source file is generated under
the working directory .

Something to be mentioned, mysql.exe must be put in system PATH . Otherwise the
CLI will complain like  "mysql is not found " .

Mysql.exe is used to connect to DB server and extract column name/type of
specified table .So information about connection is need , such as
host,port,user.etc . To make it easier to use , connection is stored in configuration file named **default.ini** . 
If default value not satisfies  your development enviroment , override the parameter in configuration file .
 
`usage : table2javabean`

Navigate to the directory where this script is put, then exceute the above
command from CLI . when prompted, type table
name ,class name . if database is not specified in configuration file , you
are asked to type it in CLI too .  you will get a XXX.java under
working directory in case that everything goes well . XXX represents for class name typed .
 
