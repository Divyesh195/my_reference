# MongoDB
## Database >> Collection >> Documents

### 1. Database level commands

```
> show dbs
> use db_name
> db.dropdatabase()
```

### 2. Collection commands
```
> db.createCollection("collection_name")

> db.getCollectionNames()

> db.collection_name.renameCollection("new_name")

> db.collection_name.drop()
```

### 3. Query commands
```
> db.collection_name.find()

> db.collection_name.findOne({name : "Divyesh"})
```

### 4. Inster data into collection
```

> db.collectionName.insertOne({name : "Divyesh Parmar", age : 20})

> db.collectionName.insertMany({name : "Divyesh Parmar", age : 20}, {name : "Daksh Parmar", age : 14})
```