### Описание:

Проект Yatube - это социальная сеть, включающая в себя следующий функционал.

# Функционал:

- **Публикации:**

    - Создание новых публикаций;
    - Получение списка всех публикаций;
    - Редактирование публикаций;
    - Удаление публикаций.

- **Группы:**

    - Получение списка всех групп;
    - Получение информации о группах.

- **Комментирии:**

    - Создание нового комментария;
    - Получение всех комментарий;
    - Получение конкретного комментария.

- **Подписка:**

    - Получение списка подписчиков;
    - Подписка на других пользователей.

### Технологии:

- Python==3.7
- Django==3.2.16
- DjangoRestFramework==3.12.4
- PyJWT==2.1.0

### Установка:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com:Yung4u/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```

### Примеры:

# Работа с API

- Первый шаг: регистрация нового пользователя
    (нужно ввести логин и пароль)
    http://127.0.0.1:8000/api/v1/auth/users/
- Второй шаг: получение JWT-токена
    (нужно ввести логин и пароль зарегистрированного пользователя)
    http://127.0.0.1:8000/api/v1/jwt/create/

После выполнения регистрации и получения токена, можно отправлять запросы вместе с токеном.

Ознакомится с полной документацией по использованию API можно по [ссылке](http://127.0.0.1:8000/redoc/)

### Автор:

[Орлов Сергей](https://github.com/Yung4u)
