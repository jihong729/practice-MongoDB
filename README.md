# practice-MongoDB

1. Install MongoDB in Mac
This is the URL for the installation process. Btw Angela's course is not up to date.
So you need to follow this path.
https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/

2. How to run MongoDB in Mac
$brew services start mongodb-community@5.0
Connect and Use MongoDB
$mongosh

*Basic command lines
$show dbs: shows the existing DBs
$use dbName: makes a new DB
$db: informs the current working DB

3. CRUD Operations
3-1: CREATE
$use nameOfDB -> this creates a DB
$db.products.insertOne({_id:1, name:"Pen", price:1.20}) -> Creating a collection called products with an entity in it.

3-2: READ
$db.collectionName.find(query, projection)
$db.products.find({price: {$gt:1}})
$db.products.find({_id:1}, {name:1, _id:0}) -> returns the data that has id of 1, but only the name value

3-3: UPDATE
$db.products.updateOne({_id:1}, {$set: {stock:32}})

3-4: DELETE
$db.products.deleteOne({_id:2})
