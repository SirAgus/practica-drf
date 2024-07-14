# Que se necesita:

-tener instalado Python y pip, pdm también.
-en la consola, instalar django con el siguiente comando: py -m pip install Django
-luego instaar drf en la consola con el siguiente comando: pip install djangorestframework

-tener los dos archivos docker-compose
-iniciar docker
-comando para iniciar los archivos docker: docker-compose --file docker-compose.dev.yml up -d
-crear proyecto django:  django-admin startproject prueba1
-crear app en django: python manage.py startapp authenticate
-instalar drf: pip install djangorestframework
-crear un superuser: pdm  django createsuperuser 
-iniciar backend: pdm dev