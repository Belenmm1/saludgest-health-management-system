medigest/
 ├── backend/          # Lógica de servidor y Base de Datos
 │   ├── main.py       # Punto de entrada de la API
 │   ├── models.py     # Definición de entidades y esquemas
 │   └── database.py   # Gestión de conexión y persistencia
 ├── frontend/         # Interfaz de Usuario (UI)
 │   ├── index.html    # Estructura del sitio
 │   └── app.js        # Lógica de cliente y consumo de API
 └── README.md
```[cite: 1]

---

## Frontend (Interfaz de Usuario)
La capa de presentación ha sido desarrollada con enfoque en la usabilidad clínica y la velocidad de respuesta.
*   **Tecnologías:** HTML5, CSS3 y JavaScript (ES6+).
*   **Lógica de Cliente (`app.js`):** Gestiona la captura de eventos, las validaciones de formularios en el lado del cliente y la comunicación asíncrona mediante `fetch`.
*   **Integración:** Consume los endpoints del backend para cargar listas de pacientes, agendar turnos y actualizar historias clínicas en tiempo real sin recargar la página.

---

##  Backend (Servidor y Datos)
El núcleo del sistema está construido en **Python**, priorizando la integridad de los datos médicos sensibles.
*   **`database.py`**: Implementa la capa de acceso a datos. Utiliza consultas SQL optimizadas para garantizar que la información de los pacientes sea accesible y segura.
*   **`models.py`**: Define las estructuras de datos (Pacientes, Médicos, Turnos) aplicando reglas de **integridad referencial** para evitar registros huérfanos o inconsistencias.
*   **`main.py`**: Orquestador principal que levanta el servicio y expone las rutas RESTful necesarias para el funcionamiento del frontend.

---

## Gestión de Base de Datos
Siguiendo los estándares de un **Analista de sistemas**, el diseño relacional incluye:
*   **Validación de Negocio:** El sistema impide la duplicidad de CUIL/DNI y asegura que no existan solapamientos en la agenda de turnos.
*   **Persistencia Atómica:** Las operaciones de escritura garantizan que los datos se guarden correctamente o se reviertan en caso de error, protegiendo el historial del paciente.

---

##  Instalación y Ejecución

### 1. Preparar el backend
```bash
cd medigest/backend
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt  # Si aplica
python main.py
```´´

### 2. Ejecutar el frontend
Simplemente abre el archivo `frontend/index.html` en un navegador o utiliza un servidor local (como Live Server) para interactuar con la API iniciada en el paso anterior.

---

**Autor:** [Maricela Belén Milde](https://belenmm1.github.io/Belenmm1/) – *Systems Analyst & Developer*.


