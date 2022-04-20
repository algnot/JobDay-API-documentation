# Check ot status
### POST <b><i>https://jobday.app/dev/v2/check_ot_status.php</i></b>
### ARGUMENTS
|Name          |Type         |Mandatory  |Description  |
|--------------|-------------|-----------|-------------|
|companyKey    |string       |YES        |             |
|email         |string       |YES        |             |
### RESPOND
|Name          |Type         |Description             |
|--------------|-------------|------------------------|
|length        |int          |number of leave status  |
|data          |array        |contain user check in   |
### Example
```js
{
  "length": 0,
  "data": []
}
```