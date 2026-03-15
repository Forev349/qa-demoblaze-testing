##Test Case 1: Successful user registration

##Тест-кейс 1: Успешная регистрация пользователя

Preconditions:
User does not have an account on the website.

Предусловия:
У пользователя нет аккаунта на сайте.

Steps:
1. Open https://www.demoblaze.com
2. Click the "Sign up" button
3. Enter a new username
4. Enter a password
5. Click the "Sign up" button

Шаги:
1. Открыть https://www.demoblaze.com
2. Нажать кнопку "Sign up"
3. Ввести новое имя пользователя
4. Ввести пароль
5. Нажать кнопку "Sign up"

Expected Result:
The user account is successfully created and a confirmation message appears.

Ожидаемый результат:
Аккаунт пользователя успешно создан и появляется сообщение о регистрации.

---

##Test Case 2: Registration with existing username

##Тест-кейс 2: Регистрация с уже существующим именем пользователя

Preconditions:
A user with this username already exists.

Предусловия:
Пользователь с таким именем уже зарегистрирован.

Steps:
 1. Open https://www.demoblaze.com
 2. Click the “Sign up” button
 3. Enter an already registered username
 4. Enter a password
 5. Click the “Sign up” button

Шаги:
 1. Открыть https://www.demoblaze.com
 2. Нажать кнопку “Sign up”
 3. Ввести уже зарегистрированное имя пользователя
 4. Ввести пароль
 5. Нажать кнопку “Sign up”

Expected Result:
The system shows an error message that the user already exists.

Ожидаемый результат:
Система показывает сообщение об ошибке, что пользователь уже существует.

---

##Test Case 3: Registration with empty fields

##Тест-кейс 3: Регистрация с пустыми полями

Preconditions:
User opens the registration form.

Предусловия:
Пользователь открыл форму регистрации.

Steps:
 1. Open https://www.demoblaze.com
 2. Click the “Sign up” button
 3. Leave the username field empty
 4. Leave the password field empty
 5. Click the “Sign up” button

Шаги:
 1. Открыть https://www.demoblaze.com
 2. Нажать кнопку “Sign up”
 3. Оставить поле username пустым
 4. Оставить поле password пустым
 5. Нажать кнопку “Sign up”

Expected Result:
The system shows a validation error message.

Ожидаемый результат:
Система показывает сообщение об ошибке валидации.
