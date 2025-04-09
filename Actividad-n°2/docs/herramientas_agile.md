# Herramientas Agile

## Tarjetas CRC

Las Tarjetas CRC (Clase, Responsabilidad, Colaborador) se utilizaron para modelar las clases principales del sistema de gestión de turnos médicos, detallando sus responsabilidades, colaboraciones, pensamiento del objeto y propiedades.

### Tarjeta CRC: Paciente

**Nombre de la Clase:** Paciente
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Sé qué especialidad necesito y mis datos personales. Quiero ver cuándo y con quién tengo turno. Necesito avisar que no podré asistir. Mis datos pueden cambiar. Quiero recordar mis visitas anteriores.
**Responsabilidades:** Solicitar un turno, Consultar sus turnos programados, Cancelar un turno, Actualizar sus datos personales, Ver el historial de sus consultas.
**Colaboradores:** Agenda, Turno, Médico.
**Propiedad:** nombre, apellido, fechaNacimiento, DNI, nroHistoriaClinica.

| Responsabilidades              | Colaboradores | Pensamiento del objeto                             |      Propiedad          |
|-------------------------       |---------------|--------------------------------------------------  |-------------------------| 
| Solicitar turno                |    Agenda     |Se qué espcialidad necesecito y mis datos personales|Nombre                   |
| Consultar turno                |    Turno      |Quiero ver cuándo y con quién tengo turno.          |Apellido                 |         
| Cancelar turno                 |    Turno      |Necesito avisar que no podré asistir.               |fechaNacimiento          |
| Actualizar sus datos personales|               |Mis datos pueden cambiar                            |DNI                      |
| Ver historial de sus consultas |Turno, Médico  |Quiero recordar mis visitas anteriores              |nroHistoriaClinica       |


![Tarjeta CRC Paciente](/Actividad-n°2/imagenes/paciente.png)

### Tarjeta CRC: Médico

**Nombre de la Clase:** Médico
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Necesito saber qué turnos tengo hoy/próximamente. Ya atendí a este paciente y debo registrar la consulta. Indicaré cuándo puedo atender pacientes. Quiero revisar el historial de este paciente.
**Responsabilidades:** Consultar su agenda de turnos, Registrar la atención de un turno, Definir su disponibilidad horaria, Ver el historial de un paciente.
**Colaboradores:** Agenda, Turno, Paciente.
**Propiedad:** nombre, apellido, especialidad, matricula.

| Responsabilidades                 | Colaboradores | Pensamiento del objeto                               |      Propiedad          |
|-----------------------------------|---------------|------------------------------------------------------|-------------------------| 
|Consultar su agenda de turnos      |Agenda, Turno  |Necesito saber qué turnos tengo hoy/próximamente      |Nombre                   |
|Registrar la atención de un turno  |Turno, Paciente|Ya atendí a este paciente y debo registrar la consulta|Apellido                 |         
|Definir su disponibilidad horaria  |Agenda         |Indicaré cuándo puedo atender pacientes               |especialidad             |
|Ver el historial de un paciente    |Paciente, Turno|Quiero revisar el historial de este paciente          |matricula                |

![Tarjeta CRC Medico](/Actividad-n°2/imagenes/medico.png)

### Tarjeta CRC: Turno

**Nombre de la Clase:** Turno
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Tengo una fecha y hora asignadas. Sé a quién debo atender. Sé quién me atenderá. Mi estado puede cambiar según la acción realizada.
**Responsabilidades:** Conocer su fecha y hora, Conocer el paciente asignado, Conocer el médico asignado, Cambiar su estado.
**Colaboradores:** Paciente, Médico, Recepcionista.
**Propiedad:** fecha, hora, estado (Pendiente, Atendido, Cancelado), motivoCancelacion (si aplica).

| Responsabilidades                 | Colaboradores       | Pensamiento del objeto                               |      Propiedad                       |
|-----------------------------------|---------------------|------------------------------------------------------|-------------------------             | 
|Conocer su fecha y hora            |                     |Tengo una fecha y hora asignadas                      |fecha                                 |
|Conocer el paciente asignado       |Paciente             |Sé a quién debo atender                               |hora                                  |         
|Conocer el médico asignado         |Médico               |Sé quién me atenderá                                  |estado(Pendiente, Atendido, Cancelado |            
|Cambiar su estado                  |Recepcionista, Médico|Mi estado puede cambiar según la acción realizada     |motivoCancelacion(si aplica)          |

![Tarjeta CRC Turno](/Actividad-n°2/imagenes/turno.png)

### Tarjeta CRC: Agenda

**Nombre de la Clase:** Agenda
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Sé cuándo y qué médicos están disponibles. Debo registrar la reserva de este paciente en este horario. Este turno ya no está disponible. Buscaré huecos libres según la especialidad y disponibilidad.
**Responsabilidades:** Mostrar la disponibilidad de turnos, Asignar un turno a un paciente, Cancelar un turno de la agenda, Buscar turnos disponibles.
**Colaboradores:** Médico, Paciente, Turno.
**Propiedad:** fechaInicio, fechaFin, medicoId, especialidadId.

| Responsabilidades                 | Colaboradores       | Pensamiento del objeto                                     |      Propiedad                      |
|-----------------------------------|---------------------|------------------------------------------------------      |-------------------------            | 
|Mostrar la disponibilidad de turnos|Médico               |Sé cuándo y qué médicos están disponibles                   |fechaInicio                          |   
|Asignar un turno a un paciente     |Paciente, Turno      |Debo registrar la reserva de este paciente en este horario  |fechaFin                             |            
|Cancelar un turno de la agenda     |Turno                |Este turno ya no está disponible                            |medicoId                             |            
|Buscar turnos disponibles          |Médico, Paciente     |Buscaré huecos libres según la especialidad y disponibilidad|especialidad                         |

![Tarjeta CRC Agenda](/Actividad-n°2/imagenes/agenda.png)

### Tarjeta CRC: Recepcionista

**Nombre de la Clase:** Recepcionista
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Necesito guardar los datos de esta persona. Este turno está confirmado para el paciente. Debo registrar la cancelación de este turno. Este paciente necesita cambiar su turno. Necesito ver la disponibilidad de este profesional.
**Responsabilidades:** Registrar un nuevo paciente, Confirmar la reserva de un turno, Cancelar un turno a solicitud, Reasignar un turno, Consultar la agenda de un médico.
**Colaboradores:** Paciente, Turno, Agenda, Médico.
**Propiedad:** nombre, apellido, usuario, password.

| Responsabilidades                 | Colaboradores       | Pensamiento del objeto                                     |      Propiedad                      |
|-----------------------------------|---------------------|------------------------------------------------------      |-------------------------            | 
|Registrar un nuevo paciente        |Paciente             |Necesito guardar los datos de esta persona                  |nombre                               |   
|Confirmar la reserva de un turno   |Turno                |Este turno está confirmado para el paciente                 |apellido                             |            
|Cancelar un turno a solicitud      |Turno                |Debo registrar la cancelación de este turno                 |usuario                              |            
|Reasignar un turno                 |Turno, Agenda        |Este paciente necesita cambiar su turno                     |password                             |                  
|Consultar la agenda de un médico   |Agenda, Médico       |Necesito ver la disponibilidad de este profesional          |                                     |

![Tarjeta CRC Recepcionista](/Actividad-n°2/imagenes/recepcionista.png)