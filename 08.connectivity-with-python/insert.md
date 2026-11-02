# insert One

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

## Insert Many

```py
student_data = [
    {
        "name": "Amit",
        "age": 21,
        "course": "Python",
        "marks": 90,
        "city": "Delhi"
    },
    {
        "name": "Priya",
        "age": 23,
        "course": "Java",
        "marks": 75,
        "city": "Noida"
    },
    {
        "name": "Rohit",
        "age": 22,
        "course": "Python",
        "marks": 65,
        "city": "Mumbai"
    }
]

result = students.insert_many(student_data)

print("Inserted IDs:", result.inserted_ids)
```

