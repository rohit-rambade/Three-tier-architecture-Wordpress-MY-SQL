# Three-tier-architecture-Wordpress-MY-SQL

With Commands : 

```docker network create --driver bridge --subnet 10.2.2.0/24 myown```


```docker run -dit --name mydb1 --network myown -e MYSQL_ROOT_PASSWORD=root@121 -e MYSQL_DATABASE=mydb -e MYSQL_USER=rohit -e MYSQL_PASSWORD=rohit@121 -v /data:/var/lib/mysql mysql```


```docker run -dit --name mywp1 -p 8080:80 --network myown wordpress```
