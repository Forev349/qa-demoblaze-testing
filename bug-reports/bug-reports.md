## BUG-REPORT 1: Registration with empty fields

## БАГ-РЕПОРТ 1: Регистрация с пустыми полями

Tiile: 
Sign up form does not validate empty required fields properly

Загалавие: 
В форме регистрации неправильно проверяются пустые обязательные поля

Environment: 
Windows 10, Yandex Browser (latest)

Окружение:
WINDOWS 10, Яндекс

Steps to reproduce:
1. Open https://www.demoblaze.com
2. Click the “Sign up” button
3. Leave the username field empty
4. Leave the password field empty
5. Click the “Sign up” button

Шаги по воспроизведению:
1. Открыть https://www.demoblaze.com
2. Нажать кнопку “Sign up”
3. Оставить поле username пустым
4. Оставить поле password пустым
5. Нажать кнопку “Sign up”

Expected result:
The system displays validation messages for required fields (username and password) and prevents form submission and does not send a request to the server

Ожидаемый результат:
Система отображает сообщения о проверке правильности заполнения обязательных полей (имя пользователя и пароль), предотвращает отправку формы и не отправляет запрос на сервер

Actual result:
System displays a generic error message instead of field-level validation messages

Актуальный результат:
Система отображает общее сообщение об ошибке вместо сообщений о проверке на уровне поля

Severity: high

Строгость: Высокая

Priority: High

Приоритет: Высокий

---

## BUG-REPORT 2: Login with empty username

## БАГ-РЕПОРТ 2: Войдите в систему с пустым именем пользователя

Tiile: 
Login API returns 500 Internal Server Error for empty username

Загалавие: 
Login API возвращает ошибку внутреннего сервера 500 для пустого имени пользователя

Environment: 
Windows 10, Yandex Browser (latest)

Окружение:
WINDOWS 10, Яндекс

Steps to reproduce:
1. Open Postman
2. Select the POST method
3. Enter the URL: https://api.demoblaze.com/login
4. Enter body: {"username":"","password":"123"}
5. Click the “Send” button

Шаги по воспроизведению:
1. Открыть Postman
2. Выбрать метод POST
3. Ввести URL: https://api.demoblaze.com/login
4. Ввести body: {"username":"","password":"123"}
5. Нажать кнопку “Send”

Expected result:
The system should return 400 Bad request for invalid input and handle request without server errors

Ожидаемый результат:
Система должна вернуть 400 (неверный запрос) на неверный ввод и обработать запрос без ошибок сервера

Actual result:
Status code: 500 Internal Server error

Актуальный результат:
Код состояния: 500 Внутренняя ошибка сервера

Severity: high

Строгость: Высокая

Priority: High

Приоритет: Высокий
