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

- $unset : remove the field from document

- $rename : rename the field

- $inc : increments the field value

- $mul : multiplies the field value

- $currentDate : Set the field Value to the current data


## Array Oprater 

- $push : add an element to an array

- $pop : remove

- $pull : remove all

- $addToSet : 




