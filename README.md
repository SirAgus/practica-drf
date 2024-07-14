# Que se necesita:

<h1>tener instalado Python y pip, pdm también.</h1>
<ul>
    <li>
        en la consola, instalar django con el siguiente comando: py -m pip install Django
    </li>
    <li>
        luego instaar drf en la consola con el siguiente comando: pip install djangorestframework
    </li>
    <li>
        tener los dos archivos docker-compose
    </li>
    <li>
        iniciar docker
    </li>
    <li>
        comando para iniciar los archivos docker: docker-compose --file docker-compose.dev.yml up -d
    </li>
    <li>
        crear proyecto django:  django-admin startproject prueba1
    </li>
    <li>
        crear app en django: python manage.py startapp authenticate
    </li>
    <li>
        instalar drf: pip install djangorestframework
    </li>
    <li>
        crear un superuser: pdm  django createsuperuser
    </li>
    <li>
        iniciar backend: pdm dev
    </li>
</ul>