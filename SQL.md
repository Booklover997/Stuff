| Command                                               | Effect                                                                           |
| ----------------------------------------------------- | -------------------------------------------------------------------------------- |
| Use {Database};                                       | Selects a database to use                                                        |
| show Databases;                                       | Shows all Databases                                                              |
| SELECT                                                | Gets information from the table does not order                                   |
| FROM                                                  | Selects what table to select for                                                 |
| ORDER BY {field} {ASC or DESC}                        | Tells the query how to order descending or ascending                             |
| WHERE                                                 | Allows to narrow the command to fields matching a condition                      |
| DISTINCT                                              | Filters out duplicates                                                           |
| {field} AS {name}                                     | A tempory name for a field to make long queries more readable or descriptive     |
| CONCAT_WS({seperator}, {firstString}, {secondString}) | Allows to catcotenate with seperator                                             |
| *                                                     | Wild card character                                                              |
| INNER JOIN                                            | Combines results from two or more tables. Condition must be true for both tables |
| describe {table};                                     | Shows the fields of a table and values they will accept                          |
| LEFT JOIN                                             | ALL from the left table as well as those that match                              |
| RIGHT JOIN                                            | Opposite of right join                                                           |
| EXISTS                                                | Check is something exists #explorefurther                                        |
| CREATE {Whatever u want to create}                    | Makes something                                                                                 |
Commonly used with [[Relational Databases]]

Allows for queries as well as [[Subqueries]]


Each field must have a datatype

| Datatype                                                     | Explanation                                                                            |
| ------------------------------------------------------------ | ---- |
| int{tinyint, longint,mediumint}(number of digits to display) | There are many types of ints to choose from and they can be [[signed]] or [[unsigned]] |
| varchar(num_of_chars)                                        | Allows for strings                                                                     |
| date                                                         | allows for the input of a date                                                                                       |

---
# Constraints
constraints allow to define the rules for a field 
```SQL
CREATE TABLE `orders` ( `orderId` mediumint(8) unsigned NOT NULL auto_increment, `date` varchar(255), `currency` varchar(255) default NULL, `total` mediumint default NULL, `customerId` mediumint unsigned NOT NULL, PRIMARY KEY (`orderId`), FOREIGN KEY (`customerId`) REFERENCES customers(`customerId`)
```


NOT NULL

Foreign Keys

Default NULL

are all examples