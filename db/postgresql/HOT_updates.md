# HOT updates in PostgreSQL

There are two conditions for HOT updates to be used:

- there must be enough space in the block containing the updated row
- there is no index defined on any column whose value it modified

Using fillfactor on tables to get HOT updates:

    ALTER TABLE mytable SET (fillfactor = 70);

Note that setting fillfactor on an existing table will not rearrange the data, it will only apply to future INSERTs. But you can use VACUUM (FULL) or CLUSTER to rewrite the table, which will respect the new fillfactor setting.

- [article on postgrespro](https://edu.postgrespro.ru/dba2/dba2_04_mvcc_hot.pdf)
- [cybertec-postgresql.com](https://www.cybertec-postgresql.com/en/hot-updates-in-postgresql-for-better-performance/)