# Logical Operators In MongoDb

> $and : Return document where both queries match

> $or : Return document where either quiry matches

> $nor : Return document where both queries fail to match

> $not : Return Documents where the query does not match

```js
// AND: both conditions must match
db.students.find({
  city: "Delhi",
  marks: { $gt: 75 }
})

// OR: either condition can match
db.students.find({
  $or: [
    { city: "Delhi" },
    { marks: { $gt: 90 } }
  ]
})

// NOR: neither condition matches
db.students.find({
  $nor: [
    { city: "Delhi" },
    { marks: { $gt: 90 } }
  ]
})

// NOT: negate a condition
db.students.find({
  age: { $not: { $gt: 20 } }
})
```
