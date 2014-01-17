table2javabean
==============
# Overview
    This tool is designed to help developer quick produce Java Bean source file
    from an exist sql table . It is implemented by dos batch and easy to use .
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
    host,port,user.etc . To make it easier to use , all of these parameters are
    hard code in script .  If default value is not satisfy your development
    enviroment , override it in script .
 
- table2javabean
  Navigate to the directory where this script is put, then exceute the above
  command from CLI . when prompted, type your database name, table
  name ,class name .etc . if everything is OK , you will get a XXX.java under
  working directory . XXX represents for class name typed .
 
- table2javabean debug
  This behaviors like  `table2javabean` command , but it also prints  tempory data  on CLI .
