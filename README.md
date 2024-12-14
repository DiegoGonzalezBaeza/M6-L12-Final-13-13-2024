# M6-L12-Final-13-13-2024
Proyecto educativo

# Install para la conexión con postgres


 ```bash
pip install psycopg2
 ```

# Settings del proyecto:

Los cambios que se deben hacer en setting.py para que se comunique con con PgAdmin.

 ```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'Blog_DB',
        'USER': 'postgres',
        'PASSWORD': 'root',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

Luego:

 ```bash
python manage.py makemigrations

python manage.py migrate
 ```