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
|status        |string       |**ok**                  |
|name          |string       |                        |
|companyKey    |string       |                        |
|email         |string       |                        |
### Example
```json
{
  "status": "ok",
  "name": "Thanawat Talabtong",
  "email": "thanawat.k2000@gmail.com",
  "key": "tongla"
}
```