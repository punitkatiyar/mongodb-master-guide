# MongoDb DataTypes

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
