---

## 📊 Especificaciones de la API
| Recurso | Método | Acción Técnica |
| :--- | :--- | :--- |
| **Pacientes** | `GET` | Recuperación indexada de expedientes[cite: 1]. |
| **Turnos** | `POST` | Registro de citas con validación de disponibilidad[cite: 1]. |
| **Historias** | `PUT` | Actualización con integridad referencial. |

---

## 🚀 Despliegue en 3 Pasos
1.  **Backend:** Ejecutar `python main.py` para levantar el servicio[cite: 1].
2.  **Frontend:** Abrir `index.html` para acceder a la interfaz reactiva[cite: 1].
3.  **Config:** Ajustar variables en `.env` para la conexión a la base de datos[cite: 1].

---

## 👩‍💻 Sobre la Autora
**Maricela Belén Milde**  
*Analista de Sistemas | Desarrolladora Full-Stack*[cite: 2].

🌍 **Portfolio:** [belenmm1.github.io/Belenmm1/](https://belenmm1.github.io/Belenmm1/)

---

### 💡 Tip para que se vea bien en GitHub:
Cuando edites el archivo en GitHub:
1. Borrá **TODO** lo que tenés ahora.
2. Pegá este nuevo código.
3. Asegurate de que el nombre del archivo sea exactamente `README.md` (en mayúsculas).
4. Hacé clic en la pestaña **"Preview"** antes de guardar para confirmar que las¡Tenes razón! Se ve así porque GitHub no está interpretando el código como formato **Markdown**, sino como texto plano. Esto pasa generalmente por dos razones: o falta una línea de espacio entre elementos, o el bloque de código de la estructura de archivos no está cerrado correctamente.

Vamos a arreglarlo de una vez. Copiá **exactamente** este bloque de abajo. He corregido los espacios y los bloques de código para que GitHub renderice las tablas y negritas correctamente.

---

# 🏥 Medigest | Enterprise Health Management System

![Status](https://img.shields.io/badge/Status-Functional-success)
![Role](https://img.shields.io/badge/Role-Systems%20Analyst-blue)
![Stack](https://img.shields.io/badge/Stack-Fullstack%20Python%2FJS-orange)

### 🎙️ Presentación Profesional
Soy **Maricela Belén Milde**, Analista de Sistemas[cite: 2]. **Medigest** es una solución de ingeniería de software diseñada para optimizar la gestión de datos en clínicas médicas[cite: 1, 3]. Mi enfoque principal fue garantizar la **trazabilidad del paciente** y la **integridad de las transacciones**.

---

## 🛠️ Ecosistema Técnico

### **Backend: Motor de Datos (Python)**
Diseñado para la robustez y seguridad de la información clínica[cite: 1].
*   **Core Logic (`main.py`):** API RESTful que orquesta las peticiones del cliente[cite: 1].
*   **Data Integrity (`models.py`):** Modelado de entidades con reglas de validación de negocio[cite: 1].
*   **Database Layer (`database.py`):** Capa de persistencia con manejo eficiente de consultas SQL.

### **Frontend: Interfaz de Usuario (JS/HTML/CSS)**
Enfoque en una UX limpia para personal administrativo[cite: 1].
*   **Reactividad:** `app.js` gestiona la comunicación asíncrona mediante `fetch`[cite: 1].
*   **Diseño:** Interfaz modular adaptada al flujo de trabajo clínico[cite: 1].

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
