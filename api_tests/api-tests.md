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
User is NOT authenticated

Actul Result:
1. Status code: 200
2. Response body: "Wrong password"

---

## API Test 3:
wrong username

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{
"username": "Gordey007", 
"password": "TWFsb3kyMDA3"
}

Expected Result:
User is NOT authenticated

Actual Result:
1. Status code: 200
2. Response body: "User does not exist."

---

## API Test 4:
empty username

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"","password":"123"}

Expected Result:
User is NOT authenticated

Actul Result:
1. Status code: 500
2. Response body: "Please fill out Username and Password"

---

API Test 5:
empty password

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"Gordey003","password":""}

Expected Result:
User is NOT authenticated

Actul Result:
1. In POSTMAN:
Response body: "Wrong password."
Status code: 200

---

API Test 6:
empty body

API Test 7:
SQL injection
