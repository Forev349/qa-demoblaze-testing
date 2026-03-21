## API Test 1:
User Login

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"testuser","password":"hash"}

Expected Result:
1. User is NOT authenticated
2. Response contains "Wrong password"

Ожидаемый результат:
1. Пользователь не прошел проверку подлинности
2. В ответе содержится сообщение "Неверный пароль"

Actul Result:
1. Status code: 200
2. Response body: "Wrong password"

Результат проверки:
1. Код состояния: 200
2. Текст ответа: "Неверный пароль"

Notes:
Request was tested using Postman

Записи:
Запрос был протестирован с помощью Postman
