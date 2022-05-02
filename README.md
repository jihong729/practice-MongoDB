# practice-MongoDB
The learning process of MongoDB

Today I learned how to...
1. Install MongoDB in Mac
This is the URL for the installation process. Btw Angela's course is not up to date.
So you need to follow this path.
https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/

2. Create new DBs and Collections in the Mongo Shell
- run the MongoDB Server
- $mongo -> which accesses the Mongo Shell
$use nameOfDB -> this creates a DB
$db.products.insertOne({_id:1, name:"Pen", price:1.20}) -> Creating a collection called products with an entity in it.
