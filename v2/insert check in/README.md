# Insert check in

### POST <b><i>https://jobday.app/dev/v2/insert_check_in.php</i></b>

<br/>

### ARGUMENTS
|Name          |Type         |Mandatory  |Description   |
|--------------|-------------|-----------|------------- |
|companyKey    |string       |YES        |              |
|email         |string       |YES        |email of user |
|status        |string       |YES        |IN or OUT only|
|date          |string       |YES        |YYYY-MM-DD    |
|time          |string       |YES        |HH:MM:SS      |
|note          |string       |YES        |              |
|location      |string       |YES        |              |

### RESPOND
|Name          |Type         |Description             |
|--------------|-------------|------------------------|
|code          |string       |**correct-password**    |
|status        |string       |                        |
|message       |string       |                        |

### Example Arguments
```json
{
    "companyKey" : "tongla",
    "email" : "thanawat.k2000@gmail.com",     
    "status" : "IN",    
    "date" : "2001-01-23",      
    "time" : "14:34:00",      
    "note" : "",      
    "location" : ""
}
```

### Example Respond
```json
{
  "code": "insert-complete",
  "name": "Thanawat Talabtong",
  "message": "insert complete"
}
```