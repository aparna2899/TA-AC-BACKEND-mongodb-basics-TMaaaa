writeCode

Write code to:-

- create a database named `sports`.
  use sports

- list all databases present in local mongod server.
  show dbs

- create 3 collections named `cricket`, `football`, `TT` in sports databse.
  db.createCollection('cricket')
  db.createCollection('football')
  db.createCollection('TT')

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
  db.cricket.insert([{name:'rahul',age:17,email:'rahul@gmail.com',bid_price:300000}])

- list all collections in sports database.
  show collections

- rename `TT` collection to `tennis`.
  db.TT.renameCollection('tennis')

- create a capped collection called `khokho` which should have max 3 documents.
  db.createCollection('khokho',{capped:true,size:10000,max:3})

  Try inserting more than 3 and see what happens?
  First inserted document gets removed.

- check whether a collection is capped or not?
  db.khokho.isCapped()

- drop all documents from `football` collection.
  db.football.drop()

- delete cricket collection completely.
  db.cricket.remove({})

- delete sports database.
  db.dropDatabase()

- check which database you are connected to ?
  sports

- connect to test database
  use test
