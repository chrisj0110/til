# Subsearches

Example of a subsearch in splunk:

```
index=my_index
| where [
    search index=my_index
    my_field = "ABC"
    | fields transaction_guid | format
]
```

The inner query will return all transaction_guid values where my_field = "ABC", and the outer query will show all events where the transaction_guid value is included in the list of values returned by the inner query.
