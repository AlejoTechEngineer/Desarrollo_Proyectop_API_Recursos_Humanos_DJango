<div align="center">

# 📌 DESARROLLO PROYECTO API RECURSOS HUMANOS DJANGO  

## 📖 Descripción

</div>

---

Este sistema proporciona una API RESTful basada en Django para la gestión de empleados, departamentos y salarios dentro de una empresa.

## 🛠️ Funcionalidades  
- Creación, edición y eliminación de empleados.  
- Asignación de empleados a departamentos específicos.  
- Control de historial salarial con fechas de actualización.  
- Seguridad con autenticación basada en tokens.  

## Arquitectura

```mermaid
flowchart TD
    A[python -m venv env] --> B[pip install -r requirements.txt]
    B --> C[Configurar variables de entorno y DB]
    C --> D[python manage.py migrate]
    D --> E[python manage.py runserver]
    E --> F[API activa en localhost:8000]
    F --> G[Swagger UI - /swagger/]
    G --> H{Operacion}
    H --> I[Empleados - models.py / views.py]
    H --> J[Departamentos - models.py / views.py]
    H --> K[Historial Salarial - models.py / views.py]
    I & J & K --> L[mi_hv_app/urls.py]
    L --> M[(db.sqlite3 / PostgreSQL)]
    M --> N[Respuesta JSON + Token Auth]
```

## 🚀 Tecnologías utilizadas  
- Django  
- Django REST Framework  
- PostgreSQL  
- Swagger para documentación de API  

## ▶️ Cómo ejecutar el proyecto  
1. Crear un entorno virtual:  
   ```bash
   python -m venv env
   source env/bin/activate  # Linux / Mac
   env\Scripts\activate  # Windows
   ```
2. Instalar dependencias:  
   ```bash
   pip install -r requirements.txt
   ```
3. Configurar las variables de entorno y base de datos.  
4. Ejecutar migraciones:  
   ```bash
   python manage.py migrate
   ```
5. Iniciar el servidor:  
   ```bash
   python manage.py runserver
   ```
6. Acceder a la documentación en `http://127.0.0.1:8000/swagger/`  

## 📌 Autor  
👨‍💻 **Alejandro De Mendoza**

---

## Autor

**Alejandro De Mendoza**  
Ingeniero Informático · Especialista en IA · Especialista en Ingeniería de Software · Máster en Arquitectura de Software

[![GitHub](https://img.shields.io/badge/GitHub-AlejoTechEngineer-181717?style=for-the-badge&logo=github)](https://github.com/AlejoTechEngineer)
