# insert document in mongoDb

## : Insert single document

```
db.users.insertOne(
  {
    name:"punit",
    course:"node",
    year:2025}
)
```
- **db.users.insertMany([{name:"punit",course:"java",year:2025},{name:"punit",course:"node",year:2025}])** : use for multiple document

- **db.users.find()** show document
  
