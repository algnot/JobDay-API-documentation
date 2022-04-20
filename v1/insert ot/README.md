# Insert ot

### POST <b><i>https://jobday.app/dev/insert_ot.php</i></b>

<br/>

### ARGUMENTS
|Name          |Type         |Mandatory  |Description  |
|--------------|-------------|-----------|-------------|
|key           |string       |YES        |api key      |
|companyKey    |string       |YES        |             |
|name          |string       |YES        |name of user |
|status        |string       |YES        |IN or OUT only|
|email         |string       |YES        |email of user|
|date          |string       |YES        |YYYY-MM-DD   |
|time          |string       |YES        |HH:MM:SS     |
|note          |string       |YES        |             |
|location      |string       |YES        |             |

### RESPOND
|Name          |Type         |Description             |
|--------------|-------------|------------------------|
|code          |string       |**200**                 |   
|status        |string       |                        |
|message       |string       |                        |
|email_send    |array        |                        |
### Example Arguments
```json
{
    "key" : "b8uPTf7dgpEKUZfS",
    "companyKey" : "tongla",
    "name" : "Thanawat Talabtong",
    "email" : "thanawat.k2000@gmail.com",     
    "date" : "2001-01-23",      
    "time" : "14:34:00",      
    "note" : "",   
    "status" : "IN",
    "location" : 3
}
```

### Example Respond
```json
{
  "code": "200",
  "status": "ok",
  "message": "insert complete"
}
```