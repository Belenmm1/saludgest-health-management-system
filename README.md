---

## 📊 Especificaciones de la API
| Recurso | Método | Acción Técnica |
| :--- | :--- | :--- |
| **Pacientes** | `GET` | Recuperación indexada de expedientes. |
| **Turnos** | `POST` | Registro de citas con validación de disponibilidad. |
| **Historias** | `PUT` | Actualización con integridad referencial. |

---

## 🚀 Despliegue en 3 Pasos
1.  **Backend:** Ejecutar `python main.py` para levantar el servicio.
2.  **Frontend:** Abrir `index.html` para acceder a la interfaz reactiva.
3.  **Config:** Ajustar variables en `.env` para la conexión a la base de datos.

---

## 👩‍💻 Sobre la Autora
**Maricela Belén Milde**  
*Analista de Sistemas*.

🌍 **Portfolio:** [belenmm1.github.io/Belenmm1/](https://belenmm1.github.io/Belenmm1/)


---

# Medigest | Enterprise Health Management System

![Status](https://img.shields.io/badge/Status-Functional-success)
![Role](https://img.shields.io/badge/Role-Systems%20Analyst-blue)
![Stack](https://img.shields.io/badge/Stack-Fullstack%20Python%2FJS-orange)


---

## Ecosistema Técnico

### **Backend: Motor de Datos (Python)**
Diseñado para la robustez y seguridad de la información clínica.
*   **Core Logic (`main.py`):** API RESTful que orquesta las peticiones del cliente.
*   **Data Integrity (`models.py`):** Modelado de entidades con reglas de validación de negocio.
*   **Database Layer (`database.py`):** Capa de persistencia con manejo eficiente de consultas SQL.

### **Frontend: Interfaz de Usuario (JS/HTML/CSS)**
Enfoque en una UX limpia para personal administrativo.
*   **Reactividad:** `app.js` gestiona la comunicación asíncrona mediante `fetch`.
*   **Diseño:** Interfaz modular adaptada al flujo de trabajo clínico.

---

## 📂 Estructura del Proyecto
```text
📦 medigest-project
 ┣ 📂 backend
 ┃ ┣ 📜 main.py         <-- API Gateway
 ┃ ┣ 📜 models.py       <-- Business Logic
 ┃ ┗ 📜 database.py     <-- Data Persistence
 ┣ 📂 frontend
 ┃ ┣ 📜 index.html      <-- Client UI
 ┃ ┗ 📜 app.js          <-- Frontend Logic
 ┗ 📜 .env.example      <-- Security Configuration
