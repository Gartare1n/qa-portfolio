### Login Request Analysis

Method: POST  
Status: 200 OK  

Valid credentials:
- Authentication successful
- User session created

Invalid credentials:
Response:
{
  "code": 2,
  "message": {
    "name": "SignInUserNotExist"
  }
}

Empty or incorrect format credential fields: 
- Nothing has been sent
- Standart error occurs

Observations:
- API returns HTTP 200 for both success and failure cases
- Error handling is implemented via response body
