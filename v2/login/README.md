# Login to use app

### POST <b><i>https://jobday.app/dev/v2/login.php</i></b>

<br/>

### ARGUMENTS
|Name          |Type         |Mandatory  |Description  |
|--------------|-------------|-----------|-------------|
|companyKey    |string       |YES        |             |
|email         |string       |YES        |             |
|password      |string       |YES        |             |
### RESPOND
|Name          |Type         |Description             |
|--------------|-------------|------------------------|
|status        |string       |                        |
|companyKey    |string       |                        |
|email         |string       |                        |
### Example
```json
{
  "status": "ok",
  "email": "kattiyanee",
  "key": "Petchco"
}
```