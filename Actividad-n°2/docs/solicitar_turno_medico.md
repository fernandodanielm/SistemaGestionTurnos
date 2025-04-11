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