# Update and Replace Document

## Update Single Document

```
db.collection.updateOne(
  {field:"value"},
  {$set:{update_field:"new value"}}
)
```

## Update Multiple Document

```
db.collection.updateMany(
  {field:"value"},
  {$set:{update_field:"new value"}}
)
```

## Update Oprater List

- $set

- $unset

- $rename

- $inc

- $mul

- $currentDate

- $min

- $max

## Array Oprater 

- $push

- $pop

- $pull

- $addToSet :




