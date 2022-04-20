
# Get user data
### POST <b><i>https://jobday.app/dev/v2/get_data.php</i></b>

### ARGUMENTS
|Name          |Type         |Mandatory  |Description  |
|--------------|-------------|-----------|-------------|
|companyKey    |string       |YES        |             |
|email         |string       |YES        |             |
|limit         |int          |YES        |             |
### RESPOND
|Name          |Type         |Description             |
|--------------|-------------|------------------------|
|user          |opject       |contain user information|
|check_in      |array        |contain user check in   |
### Example
``` json
{
  "user": {
    "name": "Thanawat Talabtong",
    "lineToken": "",
    "position": "devoloper",
    "timeIn": "09:00",
    "timeOut": ""
  },
  "check_in": [
    {
      "status": "onTime",
      "date": "2021-06-02",
      "histTimeIn": "08:00:21",
      "histTimeOut": "",
      "location": "location"
    },
    {
      "status": "late",
      "date": "2021-06-01",
      "histTimeIn": "15:11:21",
      "histTimeOut": "",
      "location": "location"
    },
    {
      "status": "late",
      "date": "2021-05-30",
      "histTimeIn": "15:11:21",
      "histTimeOut": "",
      "location": "20:11:21"
    }
  ]
}
```