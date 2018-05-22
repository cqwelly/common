## 常用命令
### 备份恢复
- mongoimport --quiet  -h 127.0.0.1:27777 -u mongodaddy -p $passwd --authenticationDatabase admin --collection collection_name -d efunds-test --upsert --file collection_name.json --drop
- mongoimport --quiet  -h 127.0.0.1:27777 -u mongodaddy -p $passwd --authenticationDatabase admin --collection collection_name -d db_name --upsert --file collection_name.json --drop
- mongoexport --quiet  -h 127.0.0.1:27777 -u mongodaddy -p $passwd --collection collection_name -d db_name -o collection_name.json


### 查询
- db.getCollection(table_name).find({'test': {"$regex": "xx$"}})
- db.getCollection('user_pdf').aggregate([{$group: {_id: '$user_name', times: {$push: '$created_at'}}}])
- db.getCollection('pdf_information').aggregate([{"$match": {"test": "test"}}, {$group: {_id: '$company_name', count: {"$sum": 1}}}, {$count: "company_name"}])

### 创建用户
- db.createUser({user: "test", pwd: "passwd", roles: [ { role: "userAdminAnyDatabase", db: "admin" } ]})
