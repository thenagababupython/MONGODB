# MONGODB
============================================================================
database-->1975--->CODD------->RDBMS.....>SQL
Example:
orcale,mysql,sqlserver,cb2 etc....


youtube------->NO SQL
EX:MONGO DB,FIRE BASE,


1.create
2.update
3.read
4.delete


curd operations:
-------------------
1.using command prompt-------dba
2.standalone applications------>testing applications
3.compare website --->for websites

oracle db:             mongo db:
---------               ---------------
database------- database
tables------collections
rows-------documents
colums---------field



create database:
====================
college
     ---->student(collections)
     name
        age
        
            address
            
INSERT:
========
mongo db:db.collection.insertOne({})
       ex:db.student.insertOne({
              name:'rajan',
              age:22,
              course:'mca',
              address: 'hyderbad'
       });
       
       naresh.insertOne({
              name:'rajan',
              age:22,
              course:'mca',
              address: 'hyderbad'
       });
       
       
       
       
  READ:
  =================
  SQL :select *  from employee
  mongo: db.student.find();
       db.student.find().pretty();--------->proper data
       select *  from employee where name='rajan'(sql)
        db.student.find({name:'rajan'}).pretty();
        
        
        
READ:
=======================================
db.student.insertMany([{},{}]);------------->insert many
db.teacher.insertMany([]);


websites for command:
================================
https://docs.mongodb.com/manual/reference/mongo-shell/

update:
=======
sql:update table 


db.teacher.updateOne(
      { "id" : 1 },
      { $set: { "first_name" : "naga","last_name":"telagarapu" } }
   );
   DELETE:
   =============
   DELETE fromemployee WHERE id 
   mongo::-->db.teacher.deleteOne({"id":2});

       
