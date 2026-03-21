## API Test 1:
Valid login

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{"username":"Gordey003","password":"hash"}

Expected Result:
The user will be registered

Actual Result:
The user has successfully logged into the account

Explanation:
You can't check it through postman because the hash is unknown

---

## API Test 2:
Wrong password

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

---

API Test 3:
wrong username

API Test 4:
empty username

API Test 5:
empty password

API Test 6:
empty body

API Test 7:
SQL injection
