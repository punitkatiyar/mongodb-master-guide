# Database => Collection => Document 

## Create Database 

- **use database_name** : create Database

- **db.dropDatabase()** : remove database

## create Collection

- **db.createCollection("students")** : create collection

- **show collections**

- **db.students.renameCollection("usres")** : rename collection

- **db.users.help()** 

- **db.users.drop()** : drop collection

## MongoDb DataTypes BSON

- String

- Double

- **32-bit Integer** 4 byte

- **64-bit Integer** 8 byte

- Boolen

- Array

- Object

- Null

- Regular Expression

- Timestamp

- Date

- ObjectId

## Example Insert Document

```
db.users.insertOne({
  name:"tester"
  age:35,
  married:false,
  dob: ISODate("2024-06-22T11:11:00Z"),
  weight:80.50,
  kids:null,
  hobbies:['sports',"movies"]
  address:{
    "street":"123 block A"
    "city":"delhi",
    "zip":201007
}
})
```


  

  
