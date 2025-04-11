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