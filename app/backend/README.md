# Backend

Este directorio contiene la aplicación backend desarrollada con Flask. Aquí está la estructura de los archivos y carpetas:

- `app/`: Código fuente de la aplicación Flask.
  - `__init__.py`: Inicialización de la aplicación y configuración de extensiones.
  - `models.py`: Definición de modelos de datos.
  - `routes.py`: Definición de rutas y controladores.
  - `config.py`: Configuración de la aplicación.
  - `templates/`: Plantillas HTML para renderización del lado del servidor (si es necesario).
  - `static/`: Archivos estáticos como CSS, JavaScript e imágenes (si es necesario).
- `migrations/`: Archivos de migraciones de la base de datos.
- `Dockerfile`: Archivo Docker para la construcción de la imagen del backend.
- `docker-compose.yml`: Archivo Docker Compose para la configuración de múltiples servicios (backend, base de datos).
- `environment.yml`: Archivo para definir el entorno Conda.
- `requirements.txt`: Archivo de requisitos para las dependencias de Python.
- `manage.py`: Script de gestión para ejecutar la aplicación.

## Instrucciones de Instalación

### Usando Conda

1. Crear y activar el entorno Conda:
```bash
conda env create -f environment.yml
conda activate myenv
```

2. Instalar dependencias adicionales:
```bash
pip install -r requirements.txt
```

3. Iniciar la aplicación:
```bash
python manage.py
```

### Usando Docker

1. Construir y ejecutar los servicios con Docker Compose:

```bash
docker-compose up --build
```

2. Acceder a la aplicación en http://localhost:5000.

## Migraciones de Base de Datos

1. Generar una nueva migración
```bash
flask db migrate -m "Mensaje de migración"
```

2. Aplicar la migración a la base de datos:
```bash
flask db upgrade
```

## Estructura del proyecto

* app/: Contiene todo el código fuente de la aplicación Flask.
  * \_\_init\_\_.py: Configuración de la aplicación, inicialización de extensiones y registro de blueprints.
  * models.py: Definición de modelos de base de datos usando SQLAlchemy.
  * routes.py: Definición de rutas y controladores.
  * config.py: Configuración de la aplicación, incluyendo la configuración de la base de datos.
  * migrations/: Directorio para las migraciones de la base de datos generadas por Flask-Migrate.
  * Dockerfile: Definición de la imagen Docker para la aplicación Flask.
  * docker-compose.yml: Definición de servicios Docker para la aplicación Flask y PostgreSQL.
  * environment.yml: Archivo de entorno para gestionar dependencias con Conda.
  * requirements.txt: Lista de dependencias de Python.
  * manage.py: Script de gestión para iniciar la aplicación y ejecutar comandos.

## Dependencias

Las principales dependencias utilizadas en este proyecto incluyen:

* Flask: Microframework para el desarrollo de aplicaciones web en Python.
* Flask-SQLAlchemy: Extensión para la integración de SQLAlchemy con Flask.
* Flask-Migrate: Extensión para el manejo de migraciones de base de datos.
* psycopg2: Adaptador de base de datos PostgreSQL para Python.

Para ver todas las dependencias, consulta el archivo `requirements.txt` y `environment.yml`.

## Configuración

* config.py: Archivo de configuración de la aplicación. Define la configuración de la base de datos y otras variables de configuración.

## Contribuir

Si tienes sugerencias o mejoras para esta plantilla, por favor contacta a los mantenedores del repositorio.

## Licencia

Este proyecto está licenciado bajo la Licencia **TODO** - ver el archivo LICENSE.md para más detalles.