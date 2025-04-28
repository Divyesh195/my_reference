# MongoDB
> Database contains collections and collection contains documents

1. To create or use database
> use db_name

2. To delete Databse 
> db.dropdatabase()

3. Create collection
> db.createCollection("collection_name")

4. All commands for collections
> db.getCollectionNames()

> db.collection_name.find()

> db.collection_name.findOne({name : "Divyesh"})

> db.collection_name.renameCollection("new_name")

> db.collection_name.drop()

5. Inster data into collection

> db.collectionName.insertOne({name : "Divyesh Parmar", age : 20})

> db.collectionName.insertMany({name : "Divyesh Parmar", age : 20}, {name : "Daksh Parmar", age : 14})