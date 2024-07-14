# Configuración del Proyecto Django con Docker y PDM

## Requisitos

### Instalaciones necesarias:
1. **Python y pip**: Asegúrate de tener Python y pip instalados.
2. **PDM**: Instala PDM para la gestión de dependencias.

## Pasos a seguir

1. **Instalar Django**:
    ```sh
    py -m pip install Django
    ```

2. **Instalar Django REST framework (DRF)**:
    ```sh
    pip install djangorestframework
    ```

3. **Archivos Docker Compose**: Asegúrate de tener los archivos `docker-compose.yml` y `docker-compose.dev.yml` en tu proyecto.
(ejemplo en los archivos: `Ejemplo_docker.txt`, `Ejemplo_docker_dev.txt` )
4. **Iniciar Docker**: Asegúrate de que Docker está ejecutándose en tu máquina.

5. **Levantar los servicios de Docker**:
    ```sh
    docker-compose --file docker-compose.dev.yml up -d
    ```

6. **Crear un proyecto Django**:
    ```sh
    django-admin startproject prueba1
    ```

7. **Crear una aplicación en Django**:
    ```sh
    python manage.py startapp authenticate
    ```

8. **Instalar DRF nuevamente si es necesario**:
    ```sh
    pip install djangorestframework
    ```

9. **Crear un superusuario en Django**:
    ```sh
    pdm run django createsuperuser
    ```

10. **Iniciar el backend**:
    ```sh
    pdm run dev
    ```

Siguiendo estos pasos, tendrás tu entorno de desarrollo configurado y listo para usar.


notas aparte: 
linter.composite = ["flake8", "ruff", "black --check", "prospector"]