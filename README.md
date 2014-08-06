J7Cache
=======

J7Cache is a high-performance in-memory database, support classes SQL, support for clusters, support for persistent data, suitable for high frequency applications and the small amount of data, such as auction systems, telecommunications pricing systems, shopping carts, order systems, online gaming platforms, stock real-time platform, the member center, log system, etc.

1、Version 0.0.2 
Release Notes: The first version of the foreign offer.
1、Support classes SQL
2、Support clustering, and support distributed deployment
3、Support persistent data to the hard disk
4、Support classes SQL

2、Brief
2.1.Start J7CacheServer
Window：X:>J7CacheServer>start.bat
Linux：>/J7CacheServer/start.sh

2.2.Supported SQL example, pay attention to keywords in uppercase,
WHERE conditions currently supports only one condition, and must
be the primary key, you can simultaneously query multiple values.

String SQL_INSERT_INTO = "INSERT INTO Test(A,B,C)
VALUES(1,ddssss,aaaa)";
String SQL_SELECT = "SELECT A,B,C FROM Test";
String SQL_UPDATE = "UPDATE Test SET B=111,C=eee WHERE A=1,2,3";
String SQL_DELETE = "DELETE FROM Test WHERE A=1";
String SQL_DROP_TABLE = "DROP TABLE Test";

2.3.Understanding the configuration file
server.properties

The machine IP: IP = 127.0.0.1
The machine service port: LOCALPORT = 7777
Cluster Service: CLUSTER = IP1: PORT, IP2: PORT
Whether persistence to disk: HDSYNC = 1
Persisted to disk interval, in seconds: HDSYNC_TIME = 10
Persistence path to the hard disk: HDSYNC_DATA_DIR = G:
/J7Cache/J7Cache_1.0.2/datas
User: USERNAME = ROOT
Passwords (MD5 encryption): PASSWORD = e10adc3949ba59abbe56e057f20f883e

2.4.Console instruction
2.4.1: Exit
Window: X:> bye!
Linux:> bye!
2.4.2 execute SQL statements, SQL statements according to the second point
of writing standards