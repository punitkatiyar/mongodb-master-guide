# Find Document

## Find All Document

```
db.collection.find()
```

## Filter Data

```
db.collection.find({city:delhi})
```

## FindOne 

```
db.collection.findOne({city:delhi})
```


## Projection

```
db.collection.find(
  { course : "node" },
  { name:1, age:1,_id:0 }
)
```
**or**

```
db.collection.find({ course : "node" }.projection({name:1,course:1,_id:0}))

```
## Projection All Data

```
db.collection.find().projection({name:1,course:1,_id:0})

```



