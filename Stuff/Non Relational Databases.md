Also known as NoSQL databases because [[SQL]] is not needed to query them unlike [[Relational Databases]] 
- Type of data is not known
- Type of data changes frequently

### Document data store
[[Json]] like format:
```json
Key: 3
Document:
{
    "firstName": "Orli",
    "lastName": "Klein",
    "address": "4981 Gravida St.",
    "city": "Barrow-in-Furness",
    "country": "United Kingdom",
    "orders": [{
        "date": "2020-09-03",
        "currency": "$",
        "total": 200,
    },
    {
        "date": "2020-11-17",
        "currency": "£",
        "total": 726,
    }]
}
```
