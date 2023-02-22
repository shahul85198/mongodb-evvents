# mongodb-evvents

### if we want to go in folder

```
    use project
```

### if we want to insert data in the folder

```
      db.events.insertOne({data})
```

### if we want to see data in the files

```
      db.events.find()
```

### if we want to read data seperatly (in many ways email and id)

```
    db.events.find({_id:objectid(1234567)}
    db.events.find({"email":"@gmail.com"})
    db.events.find({"name":"shahul"})
  
```

### if we want to update (change data)

```
      db.events.update(
      {_id:objectid(1234567)},
      {
        $set:{
              "name":"shahul",
              "email":"@gmail.com"
              }
             }
            )
 ```           
 
 ### deleting one data
 
 ```
      db.events.deletOne({_id:objectid(123456)})
      db.events.deleteOne({"name":"shahul"})
 ```
 
 ### delete all data
 
 ```
    db.events.deletemany({})
 ```   
