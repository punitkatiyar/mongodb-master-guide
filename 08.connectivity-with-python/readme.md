# setup pymongo 

> pip install pymongo

> pip show pymongo

## import PyMongo

```py
import pymongo
print(pymongo.version)
```

## MongoClient

```py
from pymongo import MongoClient
client = MongoClient("mongodb://localhost:27017/")
```


## Complete Example 

```py
from pymongo import MongoClient

client = MongoClient("mongodb://localhost:27017/")

try:
    client.admin.command("ping")
    print("MongoDB Connected Successfully!")
except Exception as e:
    print("Connection Error:", e)

```


## Getting Database and Collection

```py
from pymongo import MongoClient

client = MongoClient("mongodb://localhost:27017/")

db = client["college"]

students = db["students"]

print("Database:", db.name)
print("Collection:", students.name)

```

## Python Connectivity With MongoDB 

- Introduction to pymongo
- Installing pymongo module
- MongoClient
- Getting database and collection
- CRUD operations
- Range Queries
