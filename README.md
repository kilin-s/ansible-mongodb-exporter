# [Mongodb exporter](https://github.com/percona/mongodb_exporter)


Create user 
```
use admin

db.createUser(
   {
     user: "prometheus",
     pwd: "xxx",
     roles: [   {
         "role":"clusterMonitor",
         "db":"admin"
      },
      {
         "role":"read",
         "db":"local"
      }]
   }
)
```
