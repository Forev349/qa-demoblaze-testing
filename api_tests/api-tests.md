## API Test 1:
Valid login

Method:
POST

URL:
https://api.demoblaze.com/login

Body:
{"username":"Gordey003","password":"hash"}

Expected Result:
1. Successful account login
2. Status code: 200

Actual Result:
The user has successfully logged into the account

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
1. Status code 200
2. User is NOT authenticated

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
1. Status code: 200
2. User is NOT authenticated

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
1. Status code: 400 - validation error
2. User is NOT authenticated
3. The server should not break down

Actul Result:
1. Status code: 500
2. Response body: "Please fill out Username and Password"

Title:
Server returns 500 on empty username input

Severity:
high

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
1. Status code: 200
2. User is NOT authenticated
3. Response body: "Wrong password."

Actul Result:
1. In POSTMAN:
Response body: "Wrong password."
Status code: 200

---

API Test 6:
empty body

API Test 7:
SQL injection
