# Logout (check key matched password)

### POST <b><i>https://jobday.app/dev/v2/logout.php</i></b>

<br/>

### ARGUMENTS
|Name          |Type         |Mandatory  |Description  |
|--------------|-------------|-----------|-------------|
|companyKey    |string       |YES        |             |
|password      |string       |YES        |             |
### RESPOND
|Name          |Type         |Description             |
|--------------|-------------|------------------------|
|code          |string       |**correct-password**    |
|status        |string       |                        |
|message       |string       |                        |
### Example
**correct-password**
```json
{
  "code": "correct-password",
  "status": "correct",
  "message": "password is correct"
}
```

**wrong-password**
```json
{
  "code": "wrong-password",
  "status": "not correct",
  "message": "password is not correct"
}
```