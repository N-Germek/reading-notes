# **Databases**

## SQL and NoSQL, What are they?

1. Fill in the chart below with five differences between SQL and NoSQL databases:

|                                         SQL                                        |                                                                       NoSQL                                                                      |
|:----------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------:|
| rational                                                                           | non rational                                                                                                                                     |
| table based                                                                        | doc,key-value,graph or wide column stores                                                                                                        |
| predefined schema                                                                  | dynamic schema for unstructured data                                                                                                             |
| vertically scalable by increasing the hardware. Used to define and manipulate data | horizontally scalable by increasing the database servers the pool of resources to reduce the load                                                |
| SQL uses structured query language for defining and manipulating data              | NoSQL or UnQL uses a collection of documents and the unstructured language gives the capability to use varied syntax to match the database needs |

1. What kind of data is a good fit for an SQL database?
Data that is requires the same structure repeatedly and a developed schema would benefir the most with SQL database.
2. Give a real world example. A personal library database which has to add books to the collection would benefit with a basic schema. The tables needed to save the 
3. What kind of data is a good fit a NoSQL database? Large packages of data in varying degrees of schema or without a schema built in at all would be the best types to utilize a NoSQL database.
4. Give a real world example. A realiztic example would be for a chain grocery store's inventory. Though it is hopeful that they would utilize the same prodicts across the nation, if there are specific cpecials or products offered, a NoSQL database would be the best to maintain the information for it.
5. Which type of database is best for hierarchical data storage? A SQL database s the best for hierarchical data due to its relational data properties.
6. Which type of database is best for scalability? Depending on the needs of your app, SQL databases scale vertically and can manage increasing the load by increasing the CPU, RAM or SSD.

## SQL vs NoSQL

1. What does SQL stand for? Structured Query Language which is a language to search certain databases.

2. What is a relational database? Relational databases are databases that work with certain assumptions built in. They have presets for their data content that is strict for storage and calling methods to attain that data.

3. What type of structure does a relational database work with? Tables are a great example of structure that are rational.

4. What is a ‘schema'? The schema is the wireframe of the object that is created for the database. The fields would be the schema for the table. All records have to adhere to the schema. The purpose of the schema is to be able to reuse the same data structure similar to a wireframe over and over again with different data input in the same app.

5. What is a NoSQL database? mongoDB stems from the word humongous due to its ability to stope huge mumongous amounts of data.

6. How does it work? There are databases, yet inside the databases, there are collections, then there are documents. Due to the different structures available in collections, there is no need for a schema.

7. What is inside of a Mongo database? The Mongo database contains collections of documents and the ability to create a Schema to create and utilize the data.

8. Which is more flexible - SQL or MongoDB? and why. MongoDb is more flexible as it is able to function with more data without the strict nature of the schema. This allows it to be more dynamic as it can work with many more languages and datatypes to create the assignments.

9. What is the disadvantage of a NoSQL database? The disadvantage of NoSQL is that data changes would need to be updated in multiple documents and collections versus updating a single schema. Without a schema there isn't the ability to rely on data points to be the same without a manual build in. The read requests would be heavy since the data is usually within multiple collections and documents. The write requests would be much heavier as it may affect more files.


- > [Table Of Contents](READING-NOTES/README.md)

- > [Home Page](README.md)

## Things I want to learn more about:

### Resources

- > [SQL vs NoSQL Database Differences Explained with few Example DB](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- > [SQL vs NoSQL or MySQL vs MongoDB](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
