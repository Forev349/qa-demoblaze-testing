## API Test 1:
User Login

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"testuser","password":"123"}

Expected Result:
1. User is NOT authenticated
2. Response contains "Wrong password"

Actul Result:
1. Status code: 200
2. Response body: "Wrong password"
