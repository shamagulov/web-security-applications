# Лабораторная работа №1
> Цель работы: создание первого web приложения.
## Задание 1
1. Запустим программу:
![image](https://user-images.githubusercontent.com/82168526/149658164-617a85a6-a618-4864-ad1c-d9575b0bd940.png)
2. Модифицируем код в файле server_org.js таким образом, чтобы пользователи и пароли хранились в файле на диске.
![image](https://user-images.githubusercontent.com/82168526/149659040-b309fb84-7954-4620-b7e5-668c7d2bf562.png)
3. Заменим примитивную проверку имени и пароля в строке 18 на проверку при помощи данных из пункта 2.

![image](https://user-images.githubusercontent.com/82168526/149659061-55f501f9-c898-4166-922f-912f26d12af0.png)

4. Подберем и отдадим клиенту корректные HTTP коды в случае ошибок.

> 4.1. Если файл не найден или произошла ошибка при обработке нужно возвращать код из семейства 500.
> ![image](https://user-images.githubusercontent.com/82168526/149658250-619b2eef-653d-48bb-a88d-d236788242de.png)
>
> 4.2. Если переданы пустой пользователь или пароль, то следует возвращать код 400.
> ![image](https://user-images.githubusercontent.com/82168526/149658881-ae45f0f0-d12f-4df7-903b-ba38154aa3b6.png)
> 
> 4.3. Если переданы пользователь не найден или пароль не корректный, то следует возвращать код 403.
> ![image](https://user-images.githubusercontent.com/82168526/149658281-117264a1-ff9c-4e50-be40-47a131e008c2.png)
> ![image](https://user-images.githubusercontent.com/82168526/149658301-99bd48eb-5547-41e3-994d-b8e5abe87d3b.png)
> 
> 4.4. Если всё хорошо, то код 200.
>
>  ![image](https://user-images.githubusercontent.com/82168526/149658315-93032410-d9c2-46bd-8749-1e6bf0663a0b.png)
5. Запустим доработанный сервер node .\server_org.js и, пройдя по ссылке, http://127.0.0.1:8080/login.html убедимся, что всё работает корректно: имена и пользователи хранятся во внешнем файле.

![image](https://user-images.githubusercontent.com/82168526/149658680-b569cc79-6449-4ca6-a4c2-8f58c2c8d046.png)

![image](https://user-images.githubusercontent.com/82168526/149658497-085b3dce-59f2-4b41-ae88-75f49a4868c6.png)
