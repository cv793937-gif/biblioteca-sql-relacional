# biblioteca-sql-relacional
Base de datos relacional para una biblioteca con 6 tablas normalizadas, ERD documentado, datos de prueba y operaciones atómicas de préstamo/devolución. Incluye validación de integridad, pruebas de acciones referenciales (SET NULL, RESTRICT, CHECK) y scripts completos para reproducir el entorno.

# 📚 Library DB – Diseño Relacional Completo

Este proyecto implementa una base de datos relacional para un sistema de biblioteca.  
Incluye diseño, documentación, datos de prueba y operaciones atómicas para garantizar integridad y consistencia.

---

## 🧩 Contenido del proyecto

- **6 tablas relacionadas** (libros, autores, usuarios, membresías, préstamos, relaciones auxiliares)
- **Diagrama ERD** (dbdiagram.io, Workbench o dibujo manual)
- **15 libros** con autores (incluye un libro co-escrito)
- **7 usuarios** con diferentes tipos de membresías
- **10 préstamos** con fechas y estados
- **Operaciones atómicas**:
  - Registrar préstamo
  - Registrar devolución
  - Validación de disponibilidad
- **Pruebas de acciones referenciales**:
  - `ON DELETE SET NULL`
  - `ON DELETE RESTRICT`
  - `CHECK` constraints

---

## 🏗 Estructura del proyecto

/sql
├── schema.sql
├── inserts.sql
├── atomic_operations.sql
├── referential_tests.sql
/docs
├── ERD.png
├── diseño.md
README.md


---

## 🧪 Pruebas incluidas

- Eliminación de autores con `SET NULL`
- Bloqueo de eliminación de usuarios con préstamos activos (`RESTRICT`)
- Validación de reglas `CHECK` en membresías y préstamos
- Préstamos y devoluciones con transacciones

---

## 🚀 Objetivo del proyecto

Demostrar un diseño SQL profesional con:

- Normalización
- Integridad referencial
- Operaciones seguras
- Documentación clara
- Datos de prueba reproducibles

---

## 🐐 Créditos

Proyecto creado por **Christian**, alias *El Cabro DBA*

        |\___/|
       (  • •  )
      /   ---   \
   __/  /     \  \__
  /___/|  CABRA |___\
      LIBRARY · DB · RELACIONAL

![Diagrama ERD](documentos/ERD.png)





