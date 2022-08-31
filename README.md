# redis
## 一、数据类型
### string
```
redis 127.0.0.1:6379> SET key1 value1
redis 127.0.0.1:6379> GET key1
value1
redis 127.0.0.1:6379> DEL key1
```
### hash
```
redis 127.0.0.1:6379> HMSET hash1 field1 'v1' field2 'v2'
redis 127.0.0.1:6379> HGET hash1 field1
v1
redis 127.0.0.1:6379> HDEL hash1 field1
redis 127.0.0.1:6379> HEXISTS hash1 field1
```
### list
```
redis 127.0.0.1:6379> lpush list1 value1 value2
redis 127.0.0.1:6379> lrange list1 0 1
```
### set
set是string的无序集合
```
redis 127.0.0.1:6379> sadd set1 a
redis 127.0.0.1:6379> sadd set1 b
redis 127.0.0.1:6379> smembers set1
a
b
redis 127.0.0.1:6379> sdiff set1 set2 set3 *返回set的差集*
redis 127.0.0.1:6379>  sinter set1 set2 *返回set的交集*
redis 127.0.0.1:6379> 
```
### sorted set
有序集合
## 高可用
### 主从



