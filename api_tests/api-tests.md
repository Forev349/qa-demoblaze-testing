## API Test 1:
User Login

Method:
POST

URL: 
https://api.demoblaze.com/login

Body:
{"username":"testuser","password":"hash"}

Expected Result:
User in not authenticated
Response contains "Wrong password"

Ожидаемый результат:
Пользователь не прошел проверку подлинности
В ответе содержится сообщение "Неверный пароль"

Actul Result:
Status code: 200
Response body: "Wrong password"
Response returned successfully

Результат проверки:
Код состояния: 200
Пользователь не вошел в систему, так как пароль не правильный
Ответ возвращен успешно

Notes:
Request was tested using Postman
Backend correctly processes authentication request

Записи:
Запрос был протестирован с помощью Postman
Серверная часть корректно обрабатывает запрос на аутентификацию
