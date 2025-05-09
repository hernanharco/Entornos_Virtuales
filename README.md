
django-admin startproject webempresa

python manage.py runserver -> ejecutar

python manage.py startapp core

python manage.py createsuperuser -> configuracion del superusuario

# Para realizar migraciones 

python manage.py makemigrations / python manage.py makemigrations core

python manage.py migrate / python manage.py migrate core

# Cuando se tiene una base de datos ya creada

pip install mysqlclient -> instala mysql

python manage.py inspectdb > models.py -> Lee la base de datos existente y genera los modelos automaticamente

python manage.py inspectdb nombre_tabla > models.py -> si solo que quiere inspeccionar una tabla

# Paquetes

pip install Pillow -> paquete para la manipulacion de imagnes


# Configuracion de Entornor Virtuales

<h2>PIPENV</h2>

1.  activate django2

2. pipenv install django
   
3. pipenv run django-admin startproject webempresa

4. pipenv install -r requirements.txt

<h2>VENV</h2>

1. python -m venv venv

2. source venv/bin/activate  # En Windows: venv\Scripts\activate

3. pip install -r requirements.txt
