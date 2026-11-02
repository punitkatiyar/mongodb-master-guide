```py
student = {
    "name": "Rahul",
    "age": 22,
    "course": "Python",
    "marks": 85,
    "city": "Delhi"
}

result = students.insert_one(student)

print("Inserted ID:", result.inserted_id)
```
