# qq
qqsb、Tencentsb  
8e qqdatabase  

![Image text](https://i.imgur.com/bvstdLp.jpg)  

分享的国内网盘频繁被一些SB举报删除，数据共享人人有责  
种子 https://mega.nz/file/ct9iVLia#Zd48MrnZehsNyPd0FWX9FZ1TTc7Q9Ket-zJvboABwPw  
磁力链接 magnet:?xt=urn:btih:963fd90eee4db809ed4224d1ca7a0639c443cf4b  
magnet:?xt=urn:btih:c81e0644fd67f73d81b94a31e3fc726679638a98&dn=pcht-v1  

#使用方式：  
建立数据库，建立表 user，  
qq 的两字段 qq 和 phone，  
WB的两字段 phone 和 uid ，  
字段类型想节省空间用 bigint 就够，不然用 char 或其他。  
修改语句中的文件路径。  
语句中的 IGNORE  字段是重复数据时不覆盖，去掉就是覆盖，自行决定覆不覆盖，有重复数据不好建立唯一索引。  
还要修改mysql的配置文件，下面的语句才能执行： 在 my.ini 文件中的 mysqld 段添加 secure_file_priv=”
导入完再添加索引。  
我导入两个库分别花了二十多分钟。  
不过还是分表分库或用 nosql 吧，一个表 8e 数据，建立索引了也吃不消，mysql 单表两千万条数据左右才吃得消。  

qq8e 的导入:  
LOAD DATA INFILE ‘D:/qq_6.9_8e_update.txt’ IGNORE  
INTO TABLE `user`  
FIELDS terminated by ‘—-‘  
lines terminated by ‘\n'(qq,phone)  
WB 5e 的导入:  
LOAD DATA INFILE ‘D:/0/weibo_2019_5e.txt’ IGNORE  
INTO TABLE `user`  
FIELDS TERMINATED BY ‘\t’  
LINES TERMINATED BY ‘\n'(phone,uid)  

备用地址  
https://www.kjsv.com/
https://www.vpsche.com/10919.html  
https://www.qiqiboke.com/1041.html  

TGBOT[@shegongku58bot](https://t.me/shegongku58bot)  
[免责声明](https://github.com/qq8e/qq/blob/main/wz/%E5%85%8D%E8%B4%A3%E5%A3%B0%E6%98%8E.txt)


#Data loss#44.65GB(QQWB)BT download
大杂烩
3 年前

目前欧洲机器下载较快，不建议迅雷下载，不参与做种过程且下载速度较慢，推荐 qBittorrent 或 Transmission

UPDATE: BT支持部分文件下载，如果不需要某些裤子，在开始前取消勾选

种子链接：https://mega.nz/file/ct9iVLia#Zd … Tc7Q9Ket-zJvboABwPw

磁力链接：magnet:?xt=urn:btih:963fd90eee4db809ed4224d1ca7a0639c443cf4b

#how to use？
建立数据库，建立表 user，
qq 的两字段 qq 和 phone，
WB的两字段 phone 和 uid ，
字段类型想节省空间用 bigint 就够，不然用 char 或其他。
修改语句中的文件路径。
语句中的 IGNORE  字段是重复数据时不覆盖，去掉就是覆盖，自行决定覆不覆盖，有重复数据不好建立唯一索引。
还要修改mysql的配置文件，下面的语句才能执行： 在 my.ini 文件中的 mysqld 段添加 secure_file_priv=”
导入完再添加索引。
我导入两个库分别花了二十多分钟。
不过还是分表分库或用 nosql 吧，一个表 8e 数据，建立索引了也吃不消，mysql 单表两千万条数据左右才吃得消。

qq8e 的导入:
LOAD DATA INFILE ‘D:/qq_6.9_8e_update.txt’ IGNORE
INTO TABLE `user`
FIELDS terminated by ‘—-‘
lines terminated by ‘\n'(qq,phone)
WB 5e 的导入:
LOAD DATA INFILE ‘D:/0/weibo_2019_5e.txt’ IGNORE
INTO TABLE `user`
FIELDS TERMINATED BY ‘\t’
LINES TERMINATED BY ‘\n'(phone,uid)
