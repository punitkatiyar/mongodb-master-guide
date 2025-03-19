# insert document in mongoDb

## Insert single document

```
db.users.insertOne(
  {
    name:"punit",
    course:"node",
    year:2025}
)
```

## Insert Multiple Document 

```
db.users.insertMany(
  [
    {name:"punit",course:"java",year:2025},
    {name:"punit",course:"node",year:2025}
  ]
)
```

- **db.users.find()** show document
  
