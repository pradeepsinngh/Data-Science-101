# Relational Databases and SQL:

A database is an organized collection of data. In the past, data was stored in specialized data structures that were designed for specific tasks. 

For example, airlines might record flight bookings in a different format than a bank managing an account ledger. In 1969, Ted Codd introduced the relational model as a general method of storing data. Data is stored in two-dimensional tables called relations, consisting of individual observations in each row (commonly referred to as tuples). Each tuple is a structured data item that represents the relationship between certain attributes (columns). Each attribute of a relation has a name and data type.

A relation's schema contains its column names, data types, and constraints. A relational database can be simply described as a set of tables containing rows of individual data entries.

### Relational Database Management Systems(RDBMs):

A RDBMSs provides an interface to a relational database. Oracle, MySQL, and PostgreSQL are three of the most commonly used RDBMSs used in practice today. RDBMs give users the ability to add, edit, and remove data from databases. 

These systems provide several key benefits over using a collection of text files to store data, including:
- **Reliable data storage:** RDBMSs protect against data corruption from system failures or crashes.
- **Performance:** RDBMSs often store data more efficiently than text files and have well-developed algorithms for querying data.
- **Data management:** RDBMSs implement access control, preventing unauthorized users from accessing sensitive datasets.
- **Data consistency:** RDBMSs can impose constraints on the data entered—for example, that a column GPA only contains floats between 0.0 and 4.0.

To work with data stored in a RDBMS, we use the SQL programming language.


## RDBMS vs. pandas
### How do RDBMSs and the pandas Python package differ? 

First, pandas is not concerned about data storage. Pandas does not dictate how the data are actually stored on the underlying computer like a RDBMS does. 

Second, pandas primarily provides methods for manipulating data while RDBMSs handle both data storage and data manipulation, making them more suitable for larger datasets. A typical rule of thumb is to use a RDBMS for datasets larger than several gigabytes. 

Finally, pandas requires knowledge of Python in order to use, whereas RDBMSs require knowledge of SQL. Since SQL is simpler to learn than Python, RDBMSs allow less technical users to store and query data, a handy trait.
