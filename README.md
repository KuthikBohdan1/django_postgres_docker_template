### 🆕 Створення проєкту Django з шаблону

#### 1\. Клонування репозиторію

Для початку, склонуйте репозиторій із шаблоном собі на комп'ютер:

```bash
git clone https://github.com/KuthikBohdan1/django_postgres_docker_template
```

#### 2\. Створення нового проєкту

Перейдіть до каталогу, де ви хочете створити новий проєкт. Потім скористайтеся командою `django-admin startproject`, вказавши шлях до склонованого шаблону:

```bash
django-admin startproject --template=/шлях/до/шаблону назва_проєкту .
```

### ⚙️ Підготовка та запуск

#### 1\. Віртуальне середовище

Створіть та активуйте віртуальне середовище для ізоляції залежностей проєкту.

  * **Створення:**
    ```bash
    python -m venv .venv
    ```
  * **Активація:**
      * **Windows:**
        ```bash
        .venv\Scripts\activate
        ```
      * **Linux/macOS:**
        ```bash
        source .venv/bin/activate
        ```

#### 2\. Встановлення залежностей

Встановіть усі необхідні бібліотеки з файлу `requirements.txt`:

```bash
pip install -r requirements.txt
```

#### 3\. Міграції бази даних

Застосуйте міграції для створення необхідних таблиць у базі даних:

```bash
python manage.py makemigrations
python manage.py migrate
```

#### 4\. Створення суперкористувача

Створіть адміністратора для доступу до панелі управління Django:

```bash
python manage.py createsuperuser
```

#### 5\. Запуск сервера

Запустіть локальний сервер розробки, щоб перевірити роботу проєкту:

```bash
python manage.py runserver
```

