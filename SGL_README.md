This fork fixes a couple of issues with the upstream version:

-> The C extension wouldn't correctly extract long long values
-> The C extension wouldn't correctly pass doubles to prepared statement arguments
-> The pure-python implementation didn't handle BLOBs correctly

To build the C extension, you need the MySQL community server zip file from 
https://dev.mysql.com/downloads/mysql/ ; pass the link to it with the MYSQL_CAPI environment variable

eg MYSQL_CAPI="D:\src\mysql-8.0.25-winx64"

To install, get the libmysql.dll from the 'lib' folder of the community server zip file, as well
as the 'libcrypto' and 'libssl' .dlls from the 'bin' folder.

