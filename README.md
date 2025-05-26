
# Configuracion de Entornor Virtuales

<h2>PIPENV</h2>

1.  activate django2

2. pipenv install django
   
3. pipenv run django-admin startproject webempresa

4. pipenv install -r requirements.txt

<h2>VENV</h2>

1. python -m venv venv / py -3.12 -m venv .venv

2. source venv/bin/activate
   # En Windows:
      venv\Scripts\activate

4. pip install -r requirements.txt

_____________

# Pasos que siempre se hacen
 pip install django -> instalar DJANGO en el entorno virtual

 python manage.py makemigrations -> Crea la base de datos
 
 python manage.py migrate -> La migra

 python manage.py runserver


# Paquetes

Siempre instalar Django
pip install django

 - Hacer siempre la linea siguiente asi se evitan muchos problemas
   
      python -m pip install --upgrade pip setuptools wheel

1. pip install flask

pip install Pillow -> paquete para la manipulacion de imagnes

_______

   django-admin startproject webempresa
   django-admin startproject tapiceria_rincon_es . -> El punto . significa: "crea el proyecto en esta carpeta"." - me paso que borre el manage.py y con esto lo recupere debo estar en la carpeta principal en este caso fue tapiceria_rincon_es 

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






