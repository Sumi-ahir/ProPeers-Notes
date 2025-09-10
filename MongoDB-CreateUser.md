Day 2 - 2025-09-07

# Topic: MongoDB - Create User
### 🔹 Problem Statement
Which command in MongoDB is used to add a new user?
`db.createUser()`

### 🔹 Explanation
In MongoDB, to create a new user with specific roles, we use the **`db.createUser()`** method.  

It allows us to define:
- **username**  
- **password**  
- **roles** (permissions)

---

### 🔹 Example
```js
db.createUser({
  user: "myUser",
  pwd: "myPassword123",
  roles: [
    { role: "readWrite", db: "testDB" }
  ]
})
