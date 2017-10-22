# json interchangeable metadata structure

An experiment at defining a standard body for using json to store metadata of something.

It consists of three modules:
+ A database of standard json structure for a abstract to concrete concept, described in json format.
+ A viewer for the database, with searching query that link small word to its abstract word.
+ A validator for each language, which given an input json, it check if the json has all the desired attribute to describe a certain thing.

The structure of the database is essentially, an inheritance graph based on the directory order. The parent directory is an abstract of its child directory. Each directory has a main json with all the metadata of the abstract class. This makes it relatively easy to edit the graph manually.

The naming of the abstract need not to be absolute, as the viewer and the validator would be the ultimate resolver.

However, it's preferable if each metadata has a list of synonym.

# problem this solve

+ A single standard body to define something, so that foreign resource can validate and use.

+ This is a necessary step toward an uniform standard for distributed data, which will make it easier for people who work on data gathering to make tools for non-technical party to log data.

+ A standardized metadata for every thing in the world make it easier to validate if it is indeed that thing.

+ Farming and agriculture probably need this.

# has there been any prior work?

This is an idea log/note with bare-bone implementation. Further research is needed. If any work has been done prior, please submit an issue so this work can learn from it.

# license

MIT
