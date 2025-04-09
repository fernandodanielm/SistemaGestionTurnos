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

![Tarjeta CRC Paciente](/Actividad-n°2/imagenes/paciente.png)

### Tarjeta CRC: Médico

**Nombre de la Clase:** Médico
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Necesito saber qué turnos tengo hoy/próximamente. Ya atendí a este paciente y debo registrar la consulta. Indicaré cuándo puedo atender pacientes. Quiero revisar el historial de este paciente.
**Responsabilidades:** Consultar su agenda de turnos, Registrar la atención de un turno, Definir su disponibilidad horaria, Ver el historial de un paciente.
**Colaboradores:** Agenda, Turno, Paciente.
**Propiedad:** nombre, apellido, especialidad, matricula.

![Tarjeta CRC Medico](/Actividad-n°2/imagenes/medico.png)

### Tarjeta CRC: Turno

**Nombre de la Clase:** Turno
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Tengo una fecha y hora asignadas. Sé a quién debo atender. Sé quién me atenderá. Mi estado puede cambiar según la acción realizada.
**Responsabilidades:** Conocer su fecha y hora, Conocer el paciente asignado, Conocer el médico asignado, Cambiar su estado.
**Colaboradores:** Paciente, Médico, Recepcionista.
**Propiedad:** fecha, hora, estado (Pendiente, Atendido, Cancelado), motivoCancelacion (si aplica).

![Tarjeta CRC Turno](/Actividad-n°2/imagenes/turno.png)

### Tarjeta CRC: Agenda

**Nombre de la Clase:** Agenda
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Sé cuándo y qué médicos están disponibles. Debo registrar la reserva de este paciente en este horario. Este turno ya no está disponible. Buscaré huecos libres según la especialidad y disponibilidad.
**Responsabilidades:** Mostrar la disponibilidad de turnos, Asignar un turno a un paciente, Cancelar un turno de la agenda, Buscar turnos disponibles.
**Colaboradores:** Médico, Paciente, Turno.
**Propiedad:** fechaInicio, fechaFin, medicoId, especialidadId.

![Tarjeta CRC Agenda](/Actividad-n°2/imagenes/agenda.png)

### Tarjeta CRC: Recepcionista

**Nombre de la Clase:** Recepcionista
**Superclase:**
**Subclase:**
**Pensamiento del objeto:** Necesito guardar los datos de esta persona. Este turno está confirmado para el paciente. Debo registrar la cancelación de este turno. Este paciente necesita cambiar su turno. Necesito ver la disponibilidad de este profesional.
**Responsabilidades:** Registrar un nuevo paciente, Confirmar la reserva de un turno, Cancelar un turno a solicitud, Reasignar un turno, Consultar la agenda de un médico.
**Colaboradores:** Paciente, Turno, Agenda, Médico.
**Propiedad:** nombre, apellido, usuario, password.

![Tarjeta CRC Recepcionista](/Actividad-n°2/imagenes/recepcionista.png)