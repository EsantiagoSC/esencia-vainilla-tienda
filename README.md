# Esencia Vainilla — Tienda de postres

Aplicación web para una tienda de postres, desarrollada como proyecto de la asignatura de Bases de Datos en la Universidad Distrital Francisco José de Caldas.

Permite a los clientes registrarse, ver el catálogo, armar un carrito y hacer pedidos. Además tiene un panel de administración para gestionar productos, categorías, pedidos y usuarios.

## Tecnologías

- **Backend:** Python, FastAPI
- **Base de datos:** PostgreSQL (conexión con psycopg2)
- **Frontend:** HTML, CSS y JavaScript

## Funcionalidades

- Registro e inicio de sesión de usuarios
- Catálogo de productos por categorías
- Carrito de compras y creación de pedidos
- Historial de pedidos del cliente ("Mis pedidos")
- Panel de administración: productos, categorías, pedidos, usuarios y dashboard

## Estructura

```
app/
  models/        Modelos de datos
  repositories/  Consultas a la base de datos
  routers/       Endpoints de la API
  database.py    Conexión a PostgreSQL
  main.py        Punto de entrada
static/          Páginas, estilos, scripts e imágenes
```

## Cómo ejecutarlo

1. Crear la base de datos en PostgreSQL.
2. Copiar `.env.example` como `.env` y poner los datos de conexión.
3. Instalar dependencias:
   ```
   python -m venv venv
   venv\Scripts\activate
   pip install -r requirements.txt
   ```
4. Iniciar el servidor:
   ```
   uvicorn app.main:app --reload
   ```
5. Abrir `http://localhost:8000` en el navegador. La documentación de la API está en `http://localhost:8000/docs`.

## Autor

Edilson Santiago Sepúlveda Cortés — Estudiante de Ingeniería de Sistemas, UDFJC