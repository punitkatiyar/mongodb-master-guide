# Comparison Opraters In MongoDb

> $eq : values are equal

> $ne : Values are not equal

> $gt : Value is greater than another value

> $gte : Value is greater than or equal to another value

> $lt : value is less than another value

> $lte : value is liss than or equal to another value

> $in : value is matched within an array

> $nin : value is not matched within an array

# Example of Comparison Opraters

```
db.collectionName.find({age:{$eq:25}})
db.collectionName.find({course:{$ne:"html"}})
db.collectionName.find({age:{$gt:25}})
db.collectionName.find({age:{$gte:25}})
db.collectionName.find({age:{$lt:25}})
db.collectionName.find({age:{$lte:25}})
db.collectionName.find({age:{$in:[25,30]}})
db.collectionName.find({age:{$nin:[25,30]}})
```
