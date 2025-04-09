# Escenarios de Casos de Uso Basados en Diagramas de Flujo (Hipotéticos)

A continuación, se definirá un escenario detallado para el caso de uso "Registrar Nuevo Paciente", basado en un diagrama de flujo hipotético.

* **Caso de Uso 1 - Registrar Nuevo Paciente**
    * **Nombre del caso de uso:** Registrar Nuevo Paciente
    * **ID Única:** CU01
    * **Área:** Gestión de Pacientes
    * **Actor(es):** Recepcionista
    * **Descripción:** La recepcionista registra la información de un nuevo paciente en el sistema.
    * **Activar Evento:** La recepcionista selecciona la opción "Registrar Paciente" en la interfaz del sistema.
    * **Tipo de señal:** Externa (acción del usuario)
    * **Pasos desempeñados (ruta principal - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Muestra el formulario de registro de paciente con los campos: Nombre Completo, Número de Documento, Fecha de Nacimiento, Teléfono, Correo Electrónico.
        2.  **[Actor: Recepcionista]** Ingresa el Nombre Completo del paciente.
        3.  **[Sistema]** Valida que el campo Nombre Completo no esté vacío.
        4.  **[Actor: Recepcionista]** Ingresa el Número de Documento del paciente.
        5.  **[Sistema]** Valida el formato del Número de Documento (ej. numérico).
        6.  **[Actor: Recepcionista]** Ingresa la Fecha de Nacimiento del paciente.
        7.  **[Sistema]** Valida que la Fecha de Nacimiento sea una fecha válida.
        8.  **[Actor: Recepcionista]** Ingresa el Teléfono del paciente.
        9.  **[Sistema]** Valida el formato del Teléfono (ej. numérico).
        10. **[Actor: Recepcionista]** Ingresa el Correo Electrónico del paciente.
        11. **[Sistema]** Valida el formato del Correo Electrónico.
        12. **[Actor: Recepcionista]** Hace clic en el botón "Guardar".
        13. **[Sistema]** Verifica si ya existe un paciente con el mismo Número de Documento.
        14. **[Sistema]** Si no existe, guarda la información del paciente en la base de datos.
        15. **[Sistema]** Muestra un mensaje de "Registro Exitoso".
        16. **[Sistema]** (Opcional) Ofrece la opción de registrar otro paciente o volver al menú principal.
    * **Precondiciones:** La Recepcionista ha iniciado sesión en el sistema. La interfaz de registro de pacientes está accesible.
    * **Poscondiciones:** La información del nuevo paciente se ha guardado en la base de datos. El sistema muestra una confirmación al usuario.
    * **Suposiciones:** El sistema está conectado a la base de datos. Las reglas de validación para los campos están definidas.
    * **Reunir requerimientos:** Permitir el ingreso de la información demográfica básica del paciente. Validar la información ingresada. Almacenar la información del paciente de forma segura. Proporcionar retroalimentación al usuario sobre el éxito o el fallo del registro.
    * **Aspectos sobresalientes:** ¿Cómo se manejarán los errores de validación? ¿Se deben implementar campos opcionales? ¿Se debe generar un ID único para el paciente automáticamente?
    * **Prioridad:** Alta
    * **Riesgo:** Bajo

    * **Caso de Uso 2 - Solicitar Turno**
    * **Nombre del caso de uso:** Solicitar Turno
    * **ID Única:** CU02
    * **Área:** Gestión de Turnos
    * **Actor(es):** Paciente
    * **Descripción:** Un paciente solicita un nuevo turno médico especificando la especialidad y, opcionalmente, el médico de su preferencia.
    * **Activar Evento:** El paciente accede a la funcionalidad de solicitud de turno a través de la interfaz del sistema.
    * **Tipo de señal:** Externa (acción del usuario)
    * **Pasos desempeñados (ruta principal - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Muestra la lista de especialidades médicas disponibles.
        2.  **[Actor: Paciente]** Selecciona una especialidad.
        3.  **[Sistema]** (Opcional) Muestra la lista de médicos para la especialidad seleccionada.
        4.  **[Actor: Paciente]** (Opcional) Selecciona un médico.
        5.  **[Sistema]** Muestra un calendario con las fechas disponibles.
        6.  **[Actor: Paciente]** Selecciona una fecha.
        7.  **[Sistema]** Muestra los horarios disponibles para la fecha seleccionada (y médico, si aplica).
        8.  **[Actor: Paciente]** Selecciona un horario.
        9.  **[Sistema]** Solicita el motivo del turno.
        10. **[Actor: Paciente]** Ingresa el motivo del turno.
        11. **[Sistema]** Muestra un resumen de la solicitud (especialidad, médico, fecha, hora, motivo).
        12. **[Actor: Paciente]** Confirma la solicitud.
        13. **[Sistema]** Registra la solicitud de turno con estado "pendiente".
        14. **[Sistema]** Muestra un mensaje de confirmación de la solicitud.
    * **Precondiciones:** El paciente está registrado en el sistema. La información de especialidades, médicos y disponibilidad está actualizada.
    * **Poscondiciones:** Se registra una solicitud de turno pendiente en el sistema. Se muestra una confirmación al paciente.

* **Caso de Uso 3 - Asignar Turno**
    * **Nombre del caso de uso:** Asignar Turno
    * **ID Única:** CU03
    * **Área:** Gestión de Turnos
    * **Actor(es):** Recepcionista
    * **Descripción:** La recepcionista asigna un turno pendiente a un paciente con un médico y horario específicos.
    * **Activar Evento:** La recepcionista accede a la lista de solicitudes de turno pendientes.
    * **Tipo de señal:** Externa (acción del usuario)
    * **Pasos desempeñados (ruta principal - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Muestra la lista de solicitudes de turno pendientes.
        2.  **[Actor: Recepcionista]** Selecciona una solicitud de turno.
        3.  **[Sistema]** Muestra los detalles de la solicitud (paciente, motivo, preferencias).
        4.  **[Sistema]** Muestra la disponibilidad del médico solicitado (o permite seleccionar otro).
        5.  **[Actor: Recepcionista]** Selecciona un médico.
        6.  **[Sistema]** Muestra un calendario con la disponibilidad del médico.
        7.  **[Actor: Recepcionista]** Selecciona una fecha y hora disponible.
        8.  **[Sistema]** Muestra un resumen de la asignación (paciente, médico, fecha, hora).
        9.  **[Actor: Recepcionista]** Confirma la asignación.
        10. **[Sistema]** Actualiza el estado del turno a "confirmado".
        11. **[Sistema]** Envía notificación al paciente (ej. correo electrónico, SMS).
        12. **[Sistema]** Envía notificación al médico (ej. en su agenda).
        13. **[Sistema]** Muestra un mensaje de confirmación de la asignación.
    * **Precondiciones:** Existe una solicitud de turno pendiente. La información de médicos y su disponibilidad está actualizada. La información de contacto del paciente y el médico está disponible para las notificaciones.
    * **Poscondiciones:** El turno queda asignado en el sistema. Se envían notificaciones a las partes involucradas. Se muestra una confirmación a la recepcionista.

* **Caso de Uso 4 - Cancelar Turno**
    * **Nombre del caso de uso:** Cancelar Turno
    * **ID Única:** CU04
    * **Área:** Gestión de Turnos
    * **Actor(es):** Paciente, Recepcionista
    * **Descripción:** Un paciente o un recepcionista cancela un turno médico programado.
    * **Activar Evento:** El paciente o la recepcionista solicita la cancelación de un turno.
    * **Tipo de señal:** Externa (acción del usuario)
    * **Pasos desempeñados (ruta principal - Paciente - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Autentica al paciente.
        2.  **[Sistema]** Muestra la lista de turnos del paciente.
        3.  **[Actor: Paciente]** Selecciona el turno a cancelar.
        4.  **[Sistema]** Muestra los detalles del turno y solicita confirmación de cancelación.
        5.  **[Actor: Paciente]** Confirma la cancelación.
        6.  **[Sistema]** Actualiza el estado del turno a "cancelado".
        7.  **[Sistema]** Libera la disponibilidad en la agenda del médico.
        8.  **[Sistema]** Envía notificación de cancelación al médico.
        9.  **[Sistema]** Muestra un mensaje de confirmación de cancelación al paciente.
    * **Pasos desempeñados (ruta principal - Recepcionista - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Autentica a la recepcionista.
        2.  **[Actor: Recepcionista]** Busca el turno a cancelar (por paciente, médico, fecha).
        3.  **[Sistema]** Muestra los detalles del turno.
        4.  **[Actor: Recepcionista]** Selecciona la opción "Cancelar Turno".
        5.  **[Sistema]** (Opcional) Solicita un motivo de cancelación.
        6.  **[Actor: Recepcionista]** (Opcional) Ingresa el motivo.
        7.  **[Actor: Recepcionista]** Confirma la cancelación.
        8.  **[Sistema]** Actualiza el estado del turno a "cancelado".
        9.  **[Sistema]** Libera la disponibilidad en la agenda del médico.
        10. **[Sistema]** Envía notificación de cancelación al paciente y al médico.
        11. **[Sistema]** Muestra un mensaje de confirmación de cancelación a la recepcionista.
    * **Precondiciones:** El turno existe y no ha finalizado. El actor está autenticado.
    * **Poscondiciones:** El estado del turno es "cancelado". La disponibilidad del médico se actualiza. Se envían notificaciones.

* **Caso de Uso 5 - Consultar Historial de Turnos del Paciente**
    * **Nombre del caso de uso:** Consultar Historial de Turnos del Paciente
    * **ID Única:** CU05
    * **Área:** Gestión de Pacientes
    * **Actor(es):** Paciente, Recepcionista
    * **Descripción:** Un paciente o la recepcionista consulta el registro de los turnos asociados a un paciente específico.
    * **Activar Evento:** El paciente o la recepcionista accede a la funcionalidad de consulta del historial.
    * **Tipo de señal:** Externa (acción del usuario)
    * **Pasos desempeñados (ruta principal - Paciente - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Autentica al paciente.
        2.  **[Sistema]** Recupera el historial de turnos del paciente desde la base de datos.
        3.  **[Sistema]** Muestra una lista de los turnos (fecha, hora, médico, motivo, estado).
        4.  **[Actor: Paciente]** (Opcional) Puede seleccionar un turno para ver más detalles.
        5.  **[Sistema]** (Opcional) Muestra los detalles del turno seleccionado.
    * **Pasos desempeñados (ruta principal - Recepcionista - basado en diagrama de flujo hipotético):**
        1.  **[Sistema]** Autentica a la recepcionista.
        2.  **[Actor: Recepcionista]** Busca al paciente por nombre o número de documento.
        3.  **[Sistema]** Muestra los resultados de la búsqueda.
        4.  **[Actor: Recepcionista]** Selecciona al paciente deseado.
        5.  **[Sistema]** Recupera el historial de turnos del paciente seleccionado desde la base de datos.
        6.  **[Sistema]** Muestra una lista de los turnos (fecha, hora, médico, motivo, estado).
        7.  **[Actor: Recepcionista]** (Opcional) Puede seleccionar un turno para ver más detalles.
        8.  **[Sistema]** (Opcional) Muestra los detalles del turno seleccionado.
    * **Precondiciones:** El paciente está registrado en el sistema y tiene un historial de turnos (o la recepcionista ha encontrado al paciente deseado). El actor está autenticado.
    * **Poscondiciones:** Se muestra el historial de turnos del paciente solicitado.

Estos escenarios ahora detallan los pasos de una manera que podría reflejar un diagrama de flujo, especificando las acciones del sistema y del actor en secuencia. Recuerda que estos diagramas de flujo son hipotéticos para ilustrar el concepto.

**También cree una table en md con 5 escenarios de caso de uso**

| **Nombre del caso de uso**     | Solicitar Turno Médico                    |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-001                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente solicita un turno médico.     |
| **Activar evento**             | Selección de "Solicitar Turno".           |
| **Tipo de señal**              | Externa                                   |
| **Pasos desempeñados (ruta principal)** | 1. Acceder al sistema. <br> 2. Seleccionar consulta y médico. <br> 3. Ver horarios disponibles. <br> 4. Confirmar solicitud. <br> 5. Recibir correo de confirmación. |
| **Precondiciones**             | El paciente debe estar registrado.        |
| **Poscondiciones**             | El turno queda asignado correctamente.    |
| **Suposiciones**               | El médico tiene disponibilidad.           |

| **Nombre del caso de uso**     | Cancelar Turno Médico                     |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-002                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente cancela un turno asignado.    |
| **Activar evento**             | Selección de "Cancelar Turno".            |
| **Tipo de señal**              | Externa                                   |
| **Pasos desempeñados (ruta principal)** | 1. Iniciar sesión. <br> 2. Seleccionar turno asignado. <br> 3. Opción "Cancelar Turno". <br> 4. Verificar plazo permitido. <br> 5. Recibir confirmación por correo. |
| **Precondiciones**             | El paciente debe tener un turno asignado. |
| **Poscondiciones**             | El turno queda disponible para otros.     |
| **Suposiciones**               | La cancelación se realiza con antelación. |

| **Nombre del caso de uso**     | Consultar Turnos Disponibles              |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-003                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente consulta turnos disponibles.  |
| **Activar evento**             | Selección de "Consultar Disponibilidad".  |
| **Tipo de señal**              | Externa                                   |
| **Pasos desempeñados (ruta principal)** | 1. Acceder al sistema. <br> 2. Especificar especialidad o médico. <br> 3. Mostrar horarios disponibles. |
| **Precondiciones**             | El paciente debe estar registrado.        |
| **Poscondiciones**             | Los horarios se muestran correctamente.   |
| **Suposiciones**               | Los horarios están actualizados.          |

| **Nombre del caso de uso**     | Registrar Nuevo Paciente                  |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-004                                    |
| **Área**                       | Gestión de Usuarios                       |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | Registro de nuevos pacientes.             |
| **Activar evento**             | Selección de "Registrarse".               |
| **Tipo de señal**              | Externa                                   |
| **Pasos desempeñados (ruta principal)** | 1. Completar formulario de registro. <br> 2. Validar datos ingresados. <br> 3. Crear usuario en el sistema. <br> 4. Recibir correo de confirmación. |
| **Precondiciones**             | El paciente no debe estar registrado.     |
| **Poscondiciones**             | Usuario creado exitosamente.              |
| **Suposiciones**               | Los datos son correctos y no duplicados.  |

| **Nombre del caso de uso**     | Recordatorio de Turnos                    |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-005                                    |
| **Área**                       | Comunicación con Pacientes                |
| **Actor(es)**                  | Sistema, Paciente                         |
| **Descripción**                | Envío automático de recordatorios de turnos. |
| **Activar evento**             | Programación interna del sistema.         |
| **Tipo de señal**              | Interna                                   |
| **Pasos desempeñados (ruta principal)** | 1. Identificar turnos programados. <br> 2. Generar recordatorio con los datos del turno. <br> 3. Enviar recordatorio por correo o SMS. |
| **Precondiciones**             | El paciente tiene un turno confirmado.    |
| **Poscondiciones**             | El recordatorio es enviado correctamente. |
| **Suposiciones**               | Los datos de contacto están actualizados. |