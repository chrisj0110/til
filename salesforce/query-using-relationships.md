# query using relationships

For example:

```
SELECT Account.Name, (SELECT Contact.FirstName, Contact.LastName FROM Account.Contacts) FROM Account
```

where `Contact` is the child object name, and `Contacts` is the relationship name.

From [here](https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql_relationships_understanding.htm)

