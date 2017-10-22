# json interchangeable metadata structure

An experiment at defining a standard body for using json to store metadata of something.

It consists of three modules:
+ A database of standard json structure for a abstract to concrete concept, described in json format.
+ A viewer for the database, with searching query that link small word to its abstract word.
+ A validator for each language, which given an input json, it check if the json has all the desired attribute to describe a certain thing.

The structure of the database is essentially, an inheritance graph based on the directory order. The parent directory is an abstract of its child directory. Each directory has a main json with all the metadata of the abstract class. This makes it relatively easy to edit the graph manually.

The naming of the abstract need not to be absolute, as the viewer and the validator would be the ultimate resolver.

However, it's preferable if each metadata has a list of synonym.
