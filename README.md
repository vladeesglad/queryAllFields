# queryAllFields
Query all fields is an Apex helper class that simply returns a string list of sObject fields.  

Typically, you might need to write a one-off request to pull describe information for a single sObject or .mdt  (example methods at the bottom of the class) intending to construct a query string for a database.query.

Writing these queries can be tedious, and, if the use-case does not supply you with the knowledge of the fields that need to be returned, the you need to QUERY ALL FIELDS... anyway.

I found myself writing this particular piece of code often enough that a helper class was in order.  In this particular, one set of methods provide for all, asking the single parameter of the sObject api name to return a complete list of that sObject's fields... ready to drop-in to a query-builder.
