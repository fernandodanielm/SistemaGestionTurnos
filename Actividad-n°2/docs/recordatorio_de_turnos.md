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