**Statement Based and Row Based Replication**

**Statement Based Replication :-**

1. With statement-based replication, every SQL statement(CRUD - Create, Update and Delete) that could modify data is logged on the master.
2. Then those SQL statements are replayed on the slaves against the same dataset and in the same context.

Advantages of Statement-based Replication :- 
1. There is always less data that is to be transferred between the master and the slave.
2. There is less space taken up in the update logs.
3. There is no need to deal with the row format.
4. Also, auditing the database is easy, because statements that made any changes to the data are all logged in the binary log.
