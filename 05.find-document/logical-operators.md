# Logical Operators In MongoDb

> $and : Return document where both queries match

> $or : Return document where either quiry matches

> $nor : Return document where both queries fail to match

> $not : Return Documents where the query does not match

## Create Sample Data

```py
db.employees.insertMany([
    {name: "Amit", age: 25, salary: 30000, city: "Delhi"},
    {name: "Rahul", age: 30, salary: 45000, city: "Noida"},
    {name: "Priya", age: 28, salary: 50000, city: "Delhi"},
    {name: "Neha", age: 35, salary: 60000, city: "Mumbai"}
])
```

```js
// AND: both conditions must match
db.employees.find({
  city: "Delhi",
  marks: { $gt: 75 }
})

// AND: Age greater than 25 AND salary greater than 40000
db.employees.find({
    $and: [
        {age: {$gt: 25}},
        {salary: {$gt: 40000}}
    ]
})

// OR: Employees from Delhi OR Mumbai
db.employees.find({
    $or: [
        {city: "Delhi"},
        {city: "Mumbai"}
    ]
})

// NOT: Salary is NOT greater than 40000
db.employees.find({
    salary: {$not: {$gt: 40000}}
})

// NOR: Neither Delhi nor Mumbai
db.employees.find({
    $nor: [
        {city: "Delhi"},
        {city: "Mumbai"}
    ]
})
```
