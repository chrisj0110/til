# Querying JSON columns

If your mysql table has a column that contains JSON:

```
+------------------+
| my_column        |
+------------------+
| {                |
|     "data": [    |
|         "ABC"    |
|     ]            |
| }                |
+------------------+
```

You can query `data` like this:

```
MySQL> select JSON_EXTRACT(`my_column`, '$.data') from my_table;
+--------------------------------------------+
| JSON_EXTRACT(`my_column`, '$.data')        |
+--------------------------------------------+
| ["ABC"]                                    |
| []                                         |
+--------------------------------------------+
```

If you want to get the first value (or NULL):

```
MySQL> select JSON_UNQUOTE(JSON_EXTRACT(`my_column`, '$.data')) from my_table;
+-------------------------------------------------------------+
| JSON_UNQUOTE(JSON_EXTRACT(`my_column`, '$.data[0]'))        |
+-------------------------------------------------------------+
| ABC                                                         |
| <null>                                                      |
+-------------------------------------------------------------+
```

If you want to get a count from a list you can use `JSON_LENGTH`:

```
MySQL> select JSON_LENGTH(JSON_EXTRACT(`my_column`, '$.data')) from my_table;
+--------------------------------------------+
| JSON_EXTRACT(`my_column`, '$.data')        |
+--------------------------------------------+
| 1                                          |
| 0                                          |
+--------------------------------------------+
```

