# Update Document

```py
result = students.update_one(
    {"name": "Rahul"},
    {"$set": {"marks": 95}}
)

print("Matched:", result.matched_count)
print("Modified:", result.modified_count)
```


```py
result = students.update_many(
    {"course": "Python"},
    {"$set": {"status": "Active"}}
)

print("Matched:", result.matched_count)
print("Modified:", result.modified_count)
```
