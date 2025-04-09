# Escenarios de Casos de Uso Basados en Diagramas de Caso de uso

A continuación, se definirá un escenario detallado para los 5 escenarios de caso de uso que se solicito. Además agrego captura de pantalla del formato excel, abajo de cada table echa por md.



**Table con md de 5 escenarios de caso de uso más imagen incrustrada de archivo excel, dejo los enlaces para acceder ver las imagenes del excel**
# Escenario de caso de uso 1

# Solicitar Turno Médico

## Descripción General
Este caso de uso permite a los pacientes solicitar un turno médico de manera rápida y eficiente a través del sistema. Al acceder a la plataforma, el usuario puede seleccionar la especialidad o médico deseado, visualizar horarios disponibles y confirmar la reserva del turno. El objetivo es garantizar una gestión ordenada y accesible de citas médicas, optimizando la experiencia del paciente y del centro de salud.

## Identificación del Caso de Uso
| **Nombre del caso de uso**     | Solicitar Turno Médico                    |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-001                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente solicita un turno médico.     |
| **Activar evento**             | Selección de "Solicitar Turno".           |
| **Tipo de señal**              | Externa                                   |

## Flujo de Eventos

### **Pasos desempeñados (ruta principal)**
1. **Acceder al sistema**  
   - El paciente debe contar con un usuario y contraseña válidos; el sistema solicita autenticación para garantizar seguridad.  

2. **Seleccionar consulta y médico**  
   - El paciente elige la especialidad deseada y puede recibir sugerencias basadas en su historial médico.  

3. **Ver horarios disponibles**  
   - Se presentan horarios disponibles con filtros por fecha y franja horaria, garantizando que no haya conflictos de agenda.  

4. **Confirmar solicitud**  
   - El paciente verifica todos los detalles del turno (especialidad, médico, horario) antes de confirmar; el sistema previene duplicaciones.  

5. **Recibir correo de confirmación**  
   - El sistema envía un correo con los datos del turno y opciones para cancelar o reprogramar.  

## Condiciones

| **Precondiciones**             | El paciente debe estar registrado.        |
| **Poscondiciones**             | El turno queda asignado correctamente.    |
| **Suposiciones**               | El médico tiene disponibilidad.           |

## Detalles Claves

### **Información para los pasos**
1. **Acceder al sistema:** Se requiere autenticación segura mediante credenciales de acceso.  
2. **Seleccionar consulta y médico:** Se facilitan opciones de especialidades y médicos con filtros inteligentes.  
3. **Ver horarios disponibles:** Se muestran turnos libres y opciones de fecha según disponibilidad.  
4. **Confirmar solicitud:** Validación de datos antes de la confirmación final.  
5. **Recibir correo de confirmación:** Notificación automática con detalles del turno reservado.  

### **Requisitos**
| **Reunir Requerimientos**      | El sistema debe ser seguro y rápido para la gestión de solicitudes. |
| **Aspectos sobresalientes**    | Confirmación inmediata y flexibilidad de horarios. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Fallas en el sistema pueden afectar la disponibilidad. |

## Consideraciones Finales
Este proceso agiliza la gestión de turnos médicos, reduciendo el tiempo de espera para los pacientes y optimizando la administración de citas en el centro de salud. La disponibilidad actualizada y la seguridad en la autenticación son factores esenciales para el éxito del sistema.

---


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
| **Información para los pasos** | 1. **Acceder al sistema:** El paciente debe contar con un usuario y contraseña válidos; el sistema solicita autenticación para garantizar seguridad. <br> 2. **Seleccionar consulta y médico:** El paciente elige la especialidad deseada y puede recibir sugerencias basadas en su historial médico. <br> 3. **Ver horarios disponibles:** Se presentan horarios disponibles con filtros por fecha y franja horaria, garantizando que no haya conflictos de agenda. <br> 4. **Confirmar solicitud:** El paciente verifica todos los detalles del turno (especialidad, médico, horario) antes de confirmar; el sistema previene duplicaciones. <br> 5. **Recibir correo de confirmación:** El sistema envía un correo con los datos del turno y opciones para cancelar o reprogramar. |
| **Reunir Requerimientos**      | Sistema seguro y rápido para gestionar solicitudes. |
| **Aspectos sobresalientes**    | Confirmación inmediata, flexibilidad de horarios. |
| **Prioridad**                  | Alta                                     |
| **Riesgo**                     | Fallas en el sistema pueden afectar la disponibilidad. |

![Escenario de caso de uso 1](/Actividad-n°2/imagenes/escenariocasodeuso1.png)
[Accede a OneDrive](https://1drv.ms/i/c/f2bf844ed8279638/ER48qBWQi3pArQ-2Iuh3yskBGNIqRk0BpBCrs4A12uAW3Q?e=q2zYDX)

# Escenario de caso de uso 2

# Cancelar Turno Médico

## Descripción General
Este caso de uso permite a los pacientes cancelar un turno médico previamente asignado a través del sistema de gestión de turnos. Al realizar esta acción, el turno se libera para otros pacientes, asegurando una mejor administración de la agenda médica.

## Identificación del Caso de Uso
| **Nombre del caso de uso**     | Cancelar Turno Médico                     |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-002                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente cancela un turno asignado.    |
| **Activar evento**             | Selección de "Cancelar Turno".            |
| **Tipo de señal**              | Externa                                   |

## Flujo de Eventos

### **Pasos desempeñados (ruta principal)**
1. **Iniciar sesión**  
   - El paciente accede al sistema utilizando sus credenciales válidas.  

2. **Seleccionar turno asignado**  
   - El sistema muestra el historial de turnos y el paciente elige el turno que desea cancelar.  

3. **Opción "Cancelar Turno"**  
   - El paciente confirma la acción seleccionando el botón de cancelación.  

4. **Verificar plazo permitido**  
   - El sistema valida si la solicitud de cancelación está dentro del tiempo límite permitido por la institución médica.  

5. **Recibir correo de confirmación**  
   - Se envía una notificación por correo electrónico confirmando que el turno ha sido cancelado exitosamente.  

## Condiciones

| **Precondiciones**             | El paciente debe tener un turno asignado. |
| **Poscondiciones**             | El turno queda disponible para otros.     |
| **Suposiciones**               | La cancelación se realiza con antelación. |

## Detalles Claves

### **Información para los pasos**
1. **Iniciar sesión:** Se requiere autenticación para garantizar seguridad en el sistema.  
2. **Seleccionar turno asignado:** El paciente visualiza su historial de turnos y selecciona el turno a cancelar.  
3. **Opción "Cancelar Turno":** Confirmación de cancelación con verificación de restricciones y reglas de cancelación.  
4. **Verificar plazo permitido:** Evaluación automática del tiempo de anticipación para asegurar cumplimiento de políticas de cancelación.  
5. **Recibir correo de confirmación:** Generación y envío de un correo de confirmación para mantener al paciente informado sobre la cancelación exitosa.  

### **Requisitos**
| **Reunir Requerimientos**      | El sistema debe permitir cancelaciones automáticas y enviar notificaciones al paciente. |
| **Aspectos sobresalientes**    | Confirmación instantánea, eliminación de penalizaciones innecesarias. |
| **Prioridad**                  | Media                                      |
| **Riesgo**                     | Errores en notificaciones pueden causar confusión en los pacientes. |

## Consideraciones Finales
Este proceso contribuye a una mejor organización del sistema de turnos médicos, asegurando que los turnos cancelados queden disponibles para otros pacientes. La correcta gestión de notificaciones es clave para evitar malentendidos.

---


| **Nombre del caso de uso**     | Cancelar Turno Médico                     |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-002                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente cancela un turno asignado.    |
| **Activar evento**             | Selección de "Cancelar Turno".            |
| **Tipo de señal**              | Externa                                   |
| **Pasos desempeñados (ruta principal)** | 1. Iniciar sesión. <br> 2. Seleccionar turno asignado. <br> 3. Opción "Cancelar Turno". <br> 4. Verificar plazo permitido. <br> 5. Recibir correo de confirmación. |
| **Precondiciones**             | El paciente debe tener un turno asignado. |
| **Poscondiciones**             | El turno queda disponible para otros.     |
| **Suposiciones**               | La cancelación se realiza con antelación. |
| **Información para los pasos** | 1. **Iniciar sesión:** El paciente accede al sistema utilizando sus credenciales válidas. <br> 2. **Seleccionar turno asignado:** El sistema muestra el historial de turnos y el paciente elige el turno que desea cancelar. <br> 3. **Opción "Cancelar Turno":** El paciente confirma la acción seleccionando el botón "Cancelar Turno". <br> 4. **Verificar plazo permitido:** El sistema valida si la solicitud de cancelación está dentro del tiempo límite establecido. <br> 5. **Recibir correo de confirmación:** Se envía una notificación por correo electrónico confirmando que el turno ha sido cancelado exitosamente. |
| **Reunir Requerimientos**      | Notificación automática de cancelaciones. |
| **Aspectos sobresalientes**    | Confirmación instantánea, eliminación de penalizaciones. |
| **Prioridad**                  | Media                                    |
| **Riesgo**                     | Errores en notificaciones pueden confundir a los pacientes. |

![Escenario de caso de uso 2](/Actividad-n°2/imagenes/escenariodecasodeuso2.png)
[Accede a OneDrive](https://1drv.ms/i/c/f2bf844ed8279638/EQh2hG0_watFrO_4ZKSfchcBJ7WHxeSA4Dc4eJY98p7jZA?e=EdSGEe)

# Escenario de caso de uso 3

# Consultar Turnos Disponibles

## Descripción General
Este caso de uso permite a los pacientes consultar la disponibilidad de turnos médicos a través del sistema. Al acceder, los usuarios pueden especificar la especialidad o el médico de su preferencia y visualizar los horarios disponibles en tiempo real.

## Identificación del Caso de Uso
| **Nombre del caso de uso**     | Consultar Turnos Disponibles              |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-003                                    |
| **Área**                       | Gestión de Turnos                         |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | El paciente consulta turnos disponibles.  |
| **Activar evento**             | Selección de "Consultar Disponibilidad".  |
| **Tipo de señal**              | Externa                                   |

## Flujo de Eventos

### **Pasos desempeñados (ruta principal)**
1. **Acceder al sistema**  
   - El paciente utiliza su usuario y contraseña válidos para ingresar al sistema, asegurando autenticidad y privacidad.  

2. **Especificar especialidad o médico**  
   - El paciente selecciona la especialidad requerida o el médico preferido para encontrar opciones disponibles según su necesidad.  

3. **Mostrar horarios disponibles**  
   - El sistema consulta su base de datos y presenta al paciente una lista actualizada de horarios libres para facilitar la elección.

## Condiciones

| **Precondiciones**             | El paciente debe estar registrado.        |
| **Poscondiciones**             | Los horarios se muestran correctamente.   |
| **Suposiciones**               | Los horarios están actualizados.          |

## Detalles Claves

### **Información para los pasos**
1. **Acceder al sistema:** Se garantiza autenticación segura mediante credenciales de acceso.  
2. **Especificar especialidad o médico:** Se facilita la selección con opciones predefinidas y búsqueda avanzada.  
3. **Mostrar horarios disponibles:** Se listan únicamente los turnos libres, evitando conflictos de agenda.

### **Requisitos**
| **Reunir Requerimientos**      | El sistema debe tener una base de datos actualizada con disponibilidad de turnos. |
| **Aspectos sobresalientes**    | La interfaz debe ser intuitiva y permitir al paciente una consulta rápida. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Información desactualizada podría causar confusión en la reserva de turnos. |

## Consideraciones Finales
Este proceso facilita la planificación médica del paciente al garantizar acceso rápido a la disponibilidad de turnos. La actualización constante de los datos de agenda es clave para evitar inconvenientes en la gestión de citas.  

---

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
| **Información para los pasos** | 1. **Acceder al sistema:** El paciente utiliza su usuario y contraseña válidos para ingresar al sistema, asegurando autenticidad y privacidad. <br> 2. **Especificar especialidad o médico:** El paciente selecciona la especialidad requerida o el médico preferido para encontrar opciones disponibles según su necesidad. <br> 3. **Mostrar horarios disponibles:** El sistema consulta su base de datos y presenta al paciente una lista actualizada de horarios libres para facilitar la elección. |
| **Reunir Requerimientos**      | El sistema debe tener una base de datos actualizada con disponibilidad de turnos. |
| **Aspectos sobresalientes**    | La interfaz debe ser intuitiva y permitir al paciente una consulta rápida. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Información desactualizada podría causar confusión en la reserva de turnos. |

![Escenario de caso de uso 3](/Actividad-n°2/imagenes/escenariodecasodeuso3.png)
[Accede a OneDrive](https://1drv.ms/i/c/f2bf844ed8279638/EarX62rva7lAqG0ab09ZR1gBSJSA-5lQD-KzWCMRe6whwg?e=s33yAy)

# Escenario de caso de uso 4

# Registrar Nuevo Paciente

## Descripción General
Este caso de uso permite a los pacientes registrarse en el sistema de gestión de turnos médicos para poder solicitar turnos y acceder a sus historiales médicos. El sistema garantiza que los datos ingresados sean únicos y correctos, evitando duplicaciones y errores de registro. 

## Identificación del Caso de Uso
| **Nombre del caso de uso**     | Registrar Nuevo Paciente                  |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-004                                    |
| **Área**                       | Gestión de Usuarios                       |
| **Actor(es)**                  | Paciente, Sistema                         |
| **Descripción**                | Registro de nuevos pacientes.             |
| **Activar evento**             | Selección de "Registrarse".               |
| **Tipo de señal**              | Externa                                   |

## Flujo de Eventos

### **Pasos desempeñados (ruta principal)**
1. **Completar formulario de registro**  
   - El paciente ingresa sus datos personales y de contacto en los campos requeridos, como nombre, dirección, número de teléfono y correo electrónico.  

2. **Validar datos ingresados**  
   - El sistema verifica que los datos proporcionados sean correctos, completos y que no haya duplicados en la base de datos.  

3. **Crear usuario en el sistema**  
   - El sistema genera una cuenta única para el paciente, asociando sus datos ingresados y asignando un identificador único.  

4. **Recibir correo de confirmación**  
   - El paciente recibe un correo electrónico con detalles de su registro y un enlace para activar o confirmar su cuenta.  

## Condiciones

| **Precondiciones**             | El paciente no debe estar registrado.     |
| **Poscondiciones**             | Usuario creado exitosamente.              |
| **Suposiciones**               | Los datos son correctos y no duplicados.  |

## Detalles Claves

### **Información para los pasos**
1. **Completar formulario de registro:** El sistema solicita información detallada para asegurar la correcta identificación del paciente.  
2. **Validar datos ingresados:** Se realizan comprobaciones automáticas para evitar inconsistencias o datos repetidos.  
3. **Crear usuario en el sistema:** Se asigna un identificador único y se almacenan los datos de manera segura.  
4. **Recibir correo de confirmación:** El paciente recibe instrucciones para activar su cuenta y comenzar a usar el sistema.  

### **Requisitos**
| **Reunir Requerimientos**      | El sistema debe contar con un formulario accesible y validaciones automáticas para garantizar que los datos sean únicos y correctos. |
| **Aspectos sobresalientes**    | Proceso rápido y fácil para nuevos registros; validación automática de duplicados. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Errores en el formulario o datos duplicados podrían impedir el registro exitoso. |

## Consideraciones Finales
El proceso de registro de nuevos pacientes es fundamental para el correcto funcionamiento del sistema de gestión de turnos. La validación de datos y la generación automática de cuentas permiten garantizar eficiencia y seguridad, evitando errores de duplicación y mejorando la experiencia del usuario. Además, un sistema de confirmación confiable mediante correo electrónico permite al paciente verificar su registro y obtener acceso inmediato a los servicios de turnos médicos.

---


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
| **Información para los pasos** | 1. **Completar formulario de registro:** El paciente debe ingresar sus datos personales y de contacto en los campos requeridos, como nombre, dirección, número de teléfono y correo electrónico. <br> 2. **Validar datos ingresados:** El sistema verifica que los datos proporcionados sean correctos, completos y que no haya duplicados en la base de datos. <br> 3. **Crear usuario en el sistema:** El sistema genera una cuenta única para el paciente, asociando sus datos ingresados y asignando un identificador único. <br> 4. **Recibir correo de confirmación:** El paciente recibe un correo electrónico con detalles de su registro y un enlace para activar o confirmar su cuenta. |
| **Reunir Requerimientos**      | El sistema debe contar con un formulario accesible y validaciones automáticas para garantizar que los datos sean únicos y correctos. |
| **Aspectos sobresalientes**    | Proceso rápido y fácil para nuevos registros; validación automática de duplicados. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Errores en el formulario o datos duplicados podrían impedir el registro exitoso. |

![Escenario de caso de uso 4](/Actividad-n°2/imagenes/escenariodecasodeuso4.png)
[Accede a OneDrive](https://1drv.ms/i/c/f2bf844ed8279638/EfuY2TSTpu5HuvRawNKg-gsBpEdIR5_8WKLhtz39BVUXDg?e=SYb8UA)

# Escenario de caso de uso 5

# Recordatorio de Turnos

## Descripción General
Este caso de uso permite al sistema enviar recordatorios automáticos a los pacientes sobre sus turnos médicos próximos. A través de un proceso automatizado, el sistema identifica los turnos programados, genera la notificación con los detalles del turno y la envía por correo electrónico o SMS al paciente. Esto garantiza que los pacientes recuerden sus citas y ayuda a reducir ausencias imprevistas.

## Identificación del Caso de Uso
| **Nombre del caso de uso**     | Recordatorio de Turnos                    |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-005                                    |
| **Área**                       | Comunicación con Pacientes                |
| **Actor(es)**                  | Sistema, Paciente                         |
| **Descripción**                | Envío automático de recordatorios de turnos. |
| **Activar evento**             | Programación interna del sistema.         |
| **Tipo de señal**              | Interna                                   |

## Flujo de Eventos

### **Pasos desempeñados (ruta principal)**
1. **Identificar turnos programados**  
   - El sistema revisa automáticamente la base de datos para encontrar los turnos confirmados que necesitan un recordatorio según la fecha y hora.  

2. **Generar recordatorio con los datos del turno**  
   - El sistema compila la información relevante del turno (fecha, hora, médico, especialidad) en un formato claro para el paciente.  

3. **Enviar recordatorio por correo o SMS**  
   - Se utiliza el medio de contacto registrado por el paciente (correo electrónico o SMS) para enviar el recordatorio.  

4. **Recibir correo de confirmación**  
   - El sistema registra que el recordatorio fue enviado correctamente y puede notificar al paciente con una confirmación adicional.  

## Condiciones

| **Precondiciones**             | El paciente tiene un turno confirmado.    |
| **Poscondiciones**             | El recordatorio es enviado correctamente. |
| **Suposiciones**               | Los datos de contacto están actualizados. |

## Detalles Claves

### **Información para los pasos**
1. **Identificar turnos programados:** El sistema consulta su base de datos y extrae los turnos que requieren una notificación previa.  
2. **Generar recordatorio con los datos del turno:** Se incluye fecha, horario, especialidad, médico y otros detalles importantes.  
3. **Enviar recordatorio por correo o SMS:** Se verifica el medio de contacto preferido y se envía el recordatorio al paciente.  
4. **Recibir correo de confirmación:** Se almacena la confirmación de envío y se notifica al paciente si hubo algún problema en el proceso.  

### **Requisitos**
| **Reunir Requerimientos**      | El sistema debe ser capaz de programar recordatorios automáticos basados en horarios confirmados. |
| **Aspectos sobresalientes**    | Notificaciones oportunas y confiables, con opciones de personalización según el medio de contacto. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Fallas en la programación automática podrían impactar la experiencia del paciente. |

## Consideraciones Finales
El envío de recordatorios es una función clave para mejorar la asistencia a turnos médicos y evitar olvidos por parte de los pacientes. Un sistema de notificaciones eficiente reduce la tasa de ausencias y optimiza la gestión de turnos en el centro de salud. Es importante que el sistema cuente con mecanismos de actualización de datos de contacto y verificación de entrega para evitar errores en las notificaciones.

---


| **Nombre del caso de uso**     | Recordatorio de Turnos                    |
|--------------------------------|-------------------------------------------|
| **ID única**                   | CU-005                                    |
| **Área**                       | Comunicación con Pacientes                |
| **Actor(es)**                  | Sistema, Paciente                         |
| **Descripción**                | Envío automático de recordatorios de turnos. |
| **Activar evento**             | Programación interna del sistema.         |
| **Tipo de señal**              | Interna                                   |
| **Pasos desempeñados (ruta principal)** | 1. Identificar turnos programados. <br> 2. Generar recordatorio con los datos del turno. <br> 3. Enviar recordatorio por correo o SMS. <br> 4. Recibir correo de confirmación. |
| **Precondiciones**             | El paciente tiene un turno confirmado.    |
| **Poscondiciones**             | El recordatorio es enviado correctamente. |
| **Suposiciones**               | Los datos de contacto están actualizados. |
| **Información para los pasos** | 1. **Identificar turnos programados:** El sistema revisa automáticamente la base de datos para encontrar los turnos confirmados que necesitan un recordatorio según la fecha y hora. <br> 2. **Generar recordatorio con los datos del turno:** El sistema compila la información relevante del turno (fecha, hora, médico, especialidad) en un formato claro para el paciente. <br> 3. **Enviar recordatorio por correo o SMS:** Se utiliza el medio de contacto registrado por el paciente (correo electrónico o SMS) para enviar el recordatorio. <br> 4. **Recibir correo de confirmación:** El sistema registra que el recordatorio fue enviado correctamente y puede notificar al paciente con una confirmación adicional. |
| **Reunir Requerimientos**      | El sistema debe ser capaz de programar recordatorios automáticos basados en horarios confirmados. |
| **Aspectos sobresalientes**    | Notificaciones oportunas y confiables, con opciones de personalización según el medio de contacto. |
| **Prioridad**                  | Alta                                      |
| **Riesgo**                     | Fallas en la programación automática podrían impactar la experiencia del paciente. |

![Escenario de caso de uso 5](/Actividad-n°2/imagenes/escenariodecasodeuso5.png)

[Accede a OneDrive](https://1drv.ms/i/c/f2bf844ed8279638/ERgJ2dNlCNtHkGOUXr0QT2QBDKNRBSJ33oOqt0x6PGPFnQ?e=t4R6QI)


