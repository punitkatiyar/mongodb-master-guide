```py
user=input("enter user name")

with open(user+".txt", "a") as file:
    file.write("\n"+input("Enter Your Name "))
    file.write("\n"+input("Enter Your Email "))
    file.write("\n"+input("Enter Your Course "))
    file.write("\n"+input("Enter Your City "))
```
