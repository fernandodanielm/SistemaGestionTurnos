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