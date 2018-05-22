## 常用命令
### 查询
- db.getCollection(table_name).find({'test': {"$regex": "xx$"}})

### 创建用户
- db.createUser({user: "test", pwd: "passwd", roles: [ { role: "userAdminAnyDatabase", db: "admin" } ]})
