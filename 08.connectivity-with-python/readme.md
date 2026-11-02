Python Connectivity With MongoDB 

- Introduction to pymongo
- Installing pymongo module
- MongoClient
- Getting database and collection
- CRUD operations
- Range Queries


```py
from pymongo import MongoClient

client = MongoClient("mongodb://localhost:27017/")

db = client["college"]

students = db["students"]

print("Database:", db.name)
print("Collection:", students.name)

```
