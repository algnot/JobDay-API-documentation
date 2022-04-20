# Check leave status
### POST <b><i>https://jobday.app/dev/v2/check_leave_status.php</i></b>
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
```json
{
  "length": 3,
  "data": [
    {
      "date": "2021-12-31",
      "type": "ลากิจ",
      "note": "",
      "status": "confirmed"
    },
    {
      "date": "2021-09-05",
      "type": "ลากิจ",
      "note": "",
      "status": "confirmed"
    },
    {
      "date": "2021-08-30",
      "type": "ลาป่วย",
      "note": "",
      "status": "reject"
    }
  ]
}
```