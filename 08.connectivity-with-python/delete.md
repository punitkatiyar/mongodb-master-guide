# Delete Document

```py
result = students.delete_one({
    "name": "Rahul"
})

print("Deleted:", result.deleted_count)
```


```py
result = students.delete_many({
    "city": "Delhi"
})

print("Deleted:", result.deleted_count)

```
