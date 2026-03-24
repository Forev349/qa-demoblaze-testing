## BUG-REPORT 1: Registration with empty fields

## БАГ-РЕПОРТ 1: Регистрация с пустыми полями

Tiile: 
Sign up shows incorrect validation message for empty fields

Загалавие: 
При регистрации отображается сообщение об ошибке проверки для пустых полей.

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
The system shows a validation error message.

Ожидаемый результат:
Система показывает сообщение об ошибке валидации

Actual result:
System displays a generic error message instead of validation messages for required fields

Актуальный результат:
Вместо сообщений об ошибке проверки обязательных полей система отображает общее сообщение об ошибке.

Severity: high

Строгость: Высокая

Priority: High

Приоритет: Высокий

---

## BUG-REPORT 1: Login with empty username

## БАГ-РЕПОРТ 1: Войдите в систему с пустым именем пользователя

Tiile: 
When logging in, the server returns a code of 500

Загалавие: 
При входе в систему, сервер возвращает код:500

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
1. Открыть Postman
2. Выбрать метод POST
3. Ввести URL: https://api.demoblaze.com/login
4. Ввести body: {"username":"","password":"123"}
5. Нажать кнопку “Send”

Expected result:
The system must not break down

Ожидаемый результат:
Система не должна сломаться 

Actual result:
Status code: 500 Internal Server error

Актуальный результат:
Код состояния: 500 Внутренняя ошибка сервера

Severity: high

Строгость: Высокая

Priority: High

Приоритет: Высокий
