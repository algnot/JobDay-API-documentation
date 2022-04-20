
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
    "name": "ภาณุพงศ์ บุรกิจภาชัย",
    "lineToken": "a3B1CMOYVXhhhxuKZDXHgWhNastbZdrZ7Ny62pFGvHi",
    "position": "Developer"
  },
  "check_in": [
    {
      "timeIn": "09:30",
      "timeOut": "18:30",
      "status": "OUT",
      "date": "2021-05-31",
      "location": ""
    },
    {
      "timeIn": "09:30",
      "timeOut": "18:30",
      "status": "OUT",
      "date": "2021-05-31",
      "location": ""
    },
    {
      "timeIn": "09:30",
      "timeOut": "18:30",
      "status": "OUT",
      "date": "2021-05-31",
      "location": ""
    }
  ]
}
```