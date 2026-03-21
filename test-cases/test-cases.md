## Test Case 1: Successful user registration

## Тест-кейс 1: Успешная регистрация пользователя

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
System should successfully create a new user account and show success message.

Ожидаемый результат:
Система должна успешно создать новую учетную запись пользователя и отобразить сообщение об успешном завершении.

Actual Result: System displays a successful registration message and the user account is created.


Результат: Система выводит сообщение об успешной регистрации, и учетная запись пользователя создается.

---

## Test Case 2: Registration with existing username

## Тест-кейс 2: Регистрация с уже существующим именем пользователя

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
System should show an error message indicating that the username already exists.

Ожидаемый результат:
Система должна отобразить сообщение об ошибке, указывающее на то, что имя пользователя уже существует.

Actual Result: User already exists message is displayed

Результат: Отображается сообщение "Пользователь уже существует".

---

## Test Case 3: Registration with empty fields

## Тест-кейс 3: Регистрация с пустыми полями

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
System should display validation messages for required fields. Account should not be created.

Ожидаемый результат:
Система должна отображать сообщения об ошибке проверки для обязательных полей. Учетная запись не должна быть создана

Actual Result: System displays a validation error message for empty required fields.

Результат: Система выводит сообщение об ошибке проверки для пустых обязательных полей.

---

## Test Case 4: Login with valid credentials

## Тест-кейс 4: Вход с корректными учетными данными

Preconditions:
User has a registered account on DemoBlaze.

Предусловия:
У пользователя есть зарегистрированный аккаунт на DemoBlaze.

Steps:
 1. Open https://www.demoblaze.com
 2. Click the “Log in” button
 3. Enter valid username
 4. Enter valid password
 5. Click the “Log in” button

Шаги:
 1. Открыть https://www.demoblaze.com
 2. Нажать кнопку “Log in”
 3. Ввести корректное имя пользователя
 4. Ввести корректный пароль
 5. Нажать кнопку “Log in”

Expected Result:
System should successfully log in the user and display the username in the top navigation panel.

Ожидаемый результат:
Система должна успешно авторизовать пользователя и отобразить имя пользователя в верхней панели.

Actual Result: User successfully logs into the account

Результат: Пользователь успешно входит в аккаунт

---

## Test Case 5: Login with invalid password

## Тест-кейс 5: Вход с неправильным паролем

Preconditions:
User has a registered account on DemoBlaze.

Предусловия:
У пользователя есть зарегистрированный аккаунт на DemoBlaze.

Steps:
 1. Open https://www.demoblaze.com
 2. Click the “Log in” button
 3. Enter valid username
 4. Enter invalid password
 5. Click the “Log in” button

Шаги:
 1. Открыть https://www.demoblaze.com
 2. Нажать кнопку “Log in”
 3. Ввести корректное имя пользователя
 4. Ввести неправильный пароль
 5. Нажать кнопку “Log in”

Expected Result:
System should display an error message “Wrong password”.

Ожидаемый результат:
Система дожна показывать сообщение об ошибке «Неверный пароль».

Actual Result: System displays an error message “Wrong password”.

Результат: Система отображает сообщение об ошибке «Неверный пароль».

---

## Test Case 6: Login with empty fields

## Тест-кейс 6: Вход с пустыми полями

Preconditions:
User opens the login form on DemoBlaze.

Предусловия:
Пользователь открыл форму входа на DemoBlaze.

Steps:
 1. Open https://www.demoblaze.com
 2. Click the “Log in” button
 3. Leave username field empty
 4. Leave password field empty
 5. Click the “Log in” button

Шаги:
 1. Открыть https://www.demoblaze.com
 2. Нажать кнопку “Log in”
 3. Оставить поле username пустым
 4. Оставить поле password пустым
 5. Нажать кнопку “Log in”

Expected Result:
System shows validation error messages for empty fields.

Ожидаемый результат:
Система показывает сообщения об ошибке для пустых полей.

Actual Result: System displays validation messages for required fields.

Результат: Система отображает сообщения об ошибке для обязательных полей.

---

## Test Case 7: Add product to cart

## Тест-кейс 7: Добавление товара в корзину

Preconditions:
User is logged in.

Предусловия:
Пользователь вошёл в аккаунт.

Steps:
 1. Open https://www.demoblaze.com
 2. Select a product from the homepage
 3. Click “Add to cart”
 4. Confirm the product is added

Шаги:
 1. Открыть https://www.demoblaze.com
 2. Выбрать товар на главной странице
 3. Нажать “Add to cart”
 4. Подтвердить, что товар добавлен

Expected Result:
The product should appear in the cart, and a confirmation message should be displayed.

Ожидаемый результат:
Товар должен появиться в корзине, и должно отобразиться сообщение с подтверждением.

Actual Result: The product appears in the cart, and a confirmation message is displayed

Результат: Товар отображается в корзине, появляется сообщение о добавлении

---

## Test Case 8: Remove product from cart

## Тест-кейс 8: Удаление товара из корзины

Preconditions:
User has at least one product in the cart.

Предусловия:
В корзине есть хотя бы один товар.

Steps:
 1. Open the cart page
 2. Click “Delete” next to the product
 3. Confirm the product is removed

Шаги:
 1. Открыть страницу корзины
 2. Нажать “Delete” рядом с товаром
 3. Подтвердить, что товар удалён

Expected Result:
The product should be removed from the cart, and total price should be updated.

Ожидаемый результат:
Товар должен убраться из корзины, а стоимость должна обновиться

Actual Result: The product disappears from the cart, and total price is updated

Результат: Товар исчезает из корзины, обновляется общая стоимость

---

## Test Case 9: Place an order

## Тест-кейс 9: Оформление заказа

Preconditions:
User has at least one product in the cart and is logged in.

Предусловия:
В корзине есть хотя бы один товар, пользователь вошёл в аккаунт.

Steps:
 1. Open the cart page
 2. Click “Place Order”
 3. Fill in name, country, city, credit card, month, and year
 4. Click “Purchase”

Шаги:
 1. Открыть страницу корзины
 2. Нажать “Place Order”
 3. Заполнить поля: имя, страна, город, кредитная карта, месяц, год
 4. Нажать “Purchase”

Expected Result:
Order confirmation should appear, and order ID should be generated.

Ожидаемый результат:
Появляется сообщение о подтверждении заказа, генерируется ID заказа.

Actual Result: Order confirmation appears, and order ID is generated

Результат: Появляется сообщение о подтверждении заказа, генерируется ID заказа

---

## Test Case 10: 
Login with SQL injection

## Тестовый пример 10:
Вход в систему с помощью SQL-инъекции

Preconditions: 
User is on login page

Предварительные условия: 
Пользователь находится на странице входа в систему

Steps:
1. Open https://www.demoblaze.com
2. Click "Log in"
3. Enter username:' OR 1=1 --
4. Enter password: 123
5. Click "Log in"

Шаги:
1. Откройте https://www.demoblaze.com
2. Нажмите "Войти"
3. Введите имя пользователя:' OR 1=1 --
4. Введите пароль: 123
5. Нажмите "Войти"

Expected Result:
System should not allow login and should display an error message

ожидаемый результат:
Система не должна разрешать вход в систему и должна отображать сообщение об ошибке

Actual Result: 
System displays an error message “Wrong password”.

Результат:
Система выдает сообщение об ошибке “Неверный пароль”.

---

## Test Case 11: 
XSS atack

## Тестовый пример 11:
XSS atack

Preconditions: 
User is on login page

Предварительные условия: 
Пользователь находится на странице входа в систему

Steps:
1. Open https://www.demoblaze.com
2. Click Log in/Login
3. Enter username:<script>alert(1)</script>
4. Enter password: 123
5. Click "Log in"

Шаги:
1. Откройте https://www.demoblaze.com
2. Нажмите Войти/Регистрация
3. Введите имя пользователя:<script>alert(1)</script>
4. Введите пароль: 123
5. Нажмите "Войти"

Expected Result:
System should not allow login and should display an error message

ожидаемый результат:
Система не должна разрешать вход в систему и должна отображать сообщение об ошибке

Actual Result: 
System displays an error message “Wrong password”.

Результат:
Система выдает сообщение об ошибке “Неверный пароль”.

---

## Test Case 12: 
Special characters

## Тестовый пример 12:
Специальные символы

Preconditions: 
The user is on the registration page

Предварительные условия: 
Пользователь находится на странице регистрации

Steps:
1. Open https://www.demoblaze.com
2. Click Sign up
3. Enter username:!"№;%:?*()
4. Enter password: 123
5. Click "Sign up"

Шаги:
1. Откройте https://www.demoblaze.com
2. Нажмите Регистрация
3. Введите имя пользователя:!"№;%:?*()
4. Введите пароль: 123
5. Нажмите "Регистрация"

Expected Result:
The system should not allow the registration of a user with this name

ожидаемый результат:
Система не должна дать разрешения на регистрацию пользователя с таким именем

Actual Result: 
The system displays a message that a user with that name already exists

Результат:
Система выдает сообщение, что пользователь с таким именем уже есть

---

## Test Case 13: 
Edge case

## Тестовый пример 13:
Edge case

Preconditions: 
The user is on the registration page

Предварительные условия: 
Пользователь находится на странице регистрации

Steps:
1. Open https://www.demoblaze.com
2. Click Sign up
3. Enter username: wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww
4. Enter password: 123
5. Click "Sign up"

Шаги:
1. Откройте https://www.demoblaze.com
2. Нажмите Регистрация
3. Введите имя пользователя:wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww
4. Введите пароль: 123
5. Нажмите "Регистрация"

Expected Result:
The system should not allow the registration of a user with this name

ожидаемый результат:
Система не должна дать разрешения на регистрацию пользователя с таким именем

Actual Result: 
The system has granted permission to register a user with this name. The registration was successful

Результат:
Система дала разрешения на регистрацию пользователя с таким именем. Регистрация прошла успешно
