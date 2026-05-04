📦 medigest-project
 ┣ 📂 backend
 ┃ ┣ 📜 main.py         <-- API Gateway
 ┃ ┣ 📜 models.py       <-- Business Logic
 ┃ ┗ 📜 database.py     <-- Data Persistence
 ┣ 📂 frontend
 ┃ ┣ 📜 index.html      <-- Client UI
 ┃ ┗ 📜 app.js          <-- Frontend Logic
 ┗ 📜 .env.example      <-- Security Configuration
```

---

## Especificaciones de la API
| Recurso | Método | Acción Técnica |
| :--- | :--- | :--- |
| **Pacientes** | `GET` | Recuperación indexada de expedientes. |
| **Turnos** | `POST` | Registro de citas con validación de disponibilidad. |
| **Historias** | `PUT` | Actualización de registros clínicos con integridad referencial. |

---

##  Despliegue en 3 Pasos
1.  **Backend:** Ejecutar `python main.py` para levantar el servicio de datos.
2.  **Frontend:** Servir `index.html` (interfaz reactiva).
3.  **Config:** Ajustar variables de entorno en `.env` para conexión a DB.

---

## Sobre la autora
**Maricela Belén Milde**
*Analista de Sistemas | Desarrolladora Full-Stack*.

🌍 **Portfolio:** [belenmm1.github.io/Belenmm1/](https://belenmm1.github.io/Belenmm1/)

---


