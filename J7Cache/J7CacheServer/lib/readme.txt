1������J7CacheServer
Window��X:>J7CacheServer>start.bat
Linux��/J7CacheServer/start.sh

2�����в��Կͻ���
֧�ֵ�SQL����
String SQL_CREATE_TABLE = "CREATE TABLE Test";
String SQL_INSERT_INTO = "INSERT INTO Test(A,B,C) VALUES(1,ddssss,aaaa)";
String SQL_SELECT = "SELECT A,B,C FROM Test";
String SQL_UPDATE = "UPDATE Test SET B=111,C=eee WHERE A=1";
String SQL_DELETE = "DELETE FROM Test WHERE A=1";
String SQL_DROP_TABLE = "DROP TABLE Test";


���пͻ��ˣ�
Window��X:>J7CacheServer>java -jar J7CacheTestClient.jar 127.0.0.1 7777

Linux��/J7CacheServer/java -jar J7CacheTestClient.jar 127.0.0.1 7777

�ͻ��˻��ȡ�����ļ���sql.properties����SQL������ִ�У����Ա任

3�������ļ����
server.properties

��������˿ڣ�LOCALPORT=7777
��Ⱥ����CLUSTER=IP1:PORT,IP2:PORT