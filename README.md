# Para saber si python esta instalado 

Aquí tienes varias formas de encontrar la ubicación de Python en tu PC:

📌 Método 1: Buscar directamente en el Explorador de Archivos

1. Abre el Explorador de Archivos.
2. Ve a:   
	C:\Users\TuUsuario\AppData\Local\Programs\Python
	(Reemplaza TuUsuario con tu nombre de usuario).

3. Dentro de esta carpeta, deberías ver una subcarpeta como Python310, Python311, etc., dependiendo de la versión de Python que tengas instalada.

4. Dentro de esa subcarpeta, busca el archivo python.exe. Por ejemplo:
   
	1 	C:\Users\TuUsuario\AppData\Local\Programs\Python\Python310\python.exe
__________________________________________________________

📌 Método 2: Usar el Administrador de Paquetes de Windows (Powershell)

Si usas PowerShell, puedes intentar buscar Python usando el siguiente comando:

	1 Get-Command python
 
O para Python 3:

	1 Get-Command python3
 
Esto te mostrará la ubicación del executable de Python si está instalado.

________________________________________________________

📌 Método 3: Verificar la Instalación de Python

Si aún no encuentras Python, es posible que no esté instalado. Puedes verificarlo de estas maneras:

1. Comprobar si está instalado desde el Panel de Control
 - Ve a Panel de Control > Programas y Características .
 - Busca "Python" en la lista de programas instalados.
   
2. Instalar Python si no está presente
 - Visita la página oficial de Python .
 - Descarga e instala la versión más reciente de Python.
 - Asegúrate de marcar la opción "Add Python to PATH" durante la instalación. Esto asegura que Python esté disponible globalmente en tu sistema.

____________________________________________________

📌 Método 4: Agregar Python al PATH Manualmente
Si Python está instalado pero no está en el PATH, puedes agregarlo manualmente:

 1. Buscar la ubicación de Python :
	- Usa alguno de los métodos anteriores para encontrar la carpeta donde está instalado Python (por ejemplo, C:\Users\TuUsuario\AppData\Local\Programs\Python\Python310).

 2. Agregar Python al PATH :
	- Ve a Configuración > Sistema > Acerca de > Información del sistema > Configuración avanzada del sistema > Variables de entorno .
	- En Variables del sistema , busca la variable Path y edita su valor.
	- Agrega las siguientes rutas:
C:\Users\TuUsuario\AppData\Local\Programs\Python\Python3x
C:\Users\TuUsuario\AppData\Local\Programs\Python\Python3x\Scripts
(Reemplaza Python3x con la versión que tengas, como Python310).

 3. Reinicia la terminal para que los cambios surtan efecto.
    
📌 Verificar después de configurar el PATH

Después de configurar el PATH, vuelve a abrir una nueva terminal y ejecuta:
	
 	where python
  
Ahora debería mostrarte la ubicación de Python.

¿Qué hacer si sigues sin encontrar Python?
 - Reinstala Python : Asegúrate de marcar la opción "Add Python to PATH" durante la instalación.
 - Comprueba si tienes múltiples versiones de Python : Es posible que tengas varias versiones instaladas, y solo algunas están configuradas en el PATH.

# conf_pipenv
Los pasos para configurar el entorno virtual con Pipenv

	para ejecutar la terminal de forma rapida y de ahi en adelante podemos presionar
	ctrl + alt + n

abril la terminal e instalar

	pip install autopep8

instalar pip install pipenv -> esto ayuda a crear el entorno virtual

	Instalar pipenv
		pip install pipenv
	Crear entorno + paquete
		pipenv install nombre_paquete
	Entrar al entorno
		pipenv shell
	Salir del entorno
		exit

  	para ingresar al entorno virtual le di f1 escribi pepenv y busque 
   		f1
     		pipenv	
       		busque create enviroment
	 	venv
   		version de python
     comienza la configuracion 
   		
  
- pip install numpy
- pipenv numpy -> instalar paquetes
- pipev run pip list -> se puede ver que paquete se tiene en el proyecto
- pipev uninstall numpy -> para desistalar un paquete
- pipenv --rm -> eliminar el entorno virtual

En la siguiente lección vamos a crear nuestro primero proyecto con Pipenv. 
En el minuto 8:35 veréis que os indico que debéis configurar el linting del proyecto 
en el fichero .vscode/settings.json. Antes VSC creaba una configuración específica para 
cada proyecto automáticamente en ese fichero, actualmente ya no lo hace, así que en ese 
momento del vídeo seguid las siguientes indicaciones actualizadas:

[Resumen configuración Linting de Django en VSC (pylint y plugins)](https://gist.github.com/hcosta/6e4066ad1b938c888546c5f0a9616c48)


