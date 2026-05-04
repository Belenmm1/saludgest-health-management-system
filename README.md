#  Medigest Backend: Arquitectura de Gestión Clínica

Este repositorio contiene el núcleo lógico de **Medigest**, una solución diseñada para la digitalización de flujos de trabajo médicos. El sistema implementa una arquitectura desacoplada enfocada en la persistencia de datos y la seguridad clínica.

### Arquitectura del Sistema
El backend sigue un patrón de diseño **Layered Architecture** para asegurar la mantenibilidad:
*   **`database.py`**: Capa de abstracción de datos. Gestiona el ciclo de vida de la conexión y la configuración del motor de persistencia.
*   **`models.py`**: Definición de esquemas. Implementa la lógica de entidades (Pacientes, Médicos, Historias Clínicas) con restricciones de integridad.
*   **`main.py`**: Orquestador de la API. Define los puntos de entrada (endpoints) y el procesamiento de las peticiones HTTP.

---

###  Diseño de Base de Datos
Medigest utiliza un esquema relacional que previene la redundancia:
*   **Gestión de Entidades:** Uso de Claves Primarias (PK) y Claves Foráneas (FK) para vincular turnos con pacientes y especialistas de forma unívoca.
*   **Persistencia Segura:** Implementación de consultas parametrizadas para prevenir ataques de inyección SQL.
*   **Validación de Datos:** Reglas de negocio estrictas que impiden registros duplicados o inconsistentes en la agenda médica.

---

### 📡 Especificación de la API (Endpoints)
La comunicación con el frontend (`app.js`) se realiza mediante una interfaz RESTful:

| Método | Endpoint | Acción Técnica |
| :--- | :--- | :--- |
| **GET** | `/pacientes` | Recupera el listado de pacientes mediante una consulta optimizada.
| **POST** | `/pacientes/registro` | Inserta un nuevo registro validando CUIL y datos de contacto. |
| **POST** | `/turnos/agendar` | Registra una cita médica, verificando disponibilidad en tiempo real. |
| **PUT** | `/historia/update/:id` | Actualiza la información clínica asegurando la trazabilidad del dato. |

---

### Core Tecnológico
*   **Lenguaje:** Python (Enfoque en procesamiento lógico y limpieza de código).
*   **Base de Datos:** SQLite / SQL Engine (Gestión de transacciones y estados).
*   **Frontend Integration:** Interfaz reactiva a través de `app.js` consumiendo JSON.

---

###  Despliegue Técnico
1.  **Entorno Virtual:**
    ```bash
    python -m venv venv && source venv/bin/activate
    ```
2.  **Inicialización de la DB:**
    El sistema verifica automáticamente la existencia de las tablas al arranque (`IF NOT EXISTS`) para garantizar un entorno listo para operar.
3.  **Ejecución:**
    ```bash
    python main.py
    ```

---

**Desarrollado por:** [Maricela Belén Milde](https://belenmm1.github.io/Belenmm1/) – *Systems Analyst & Developer*.

