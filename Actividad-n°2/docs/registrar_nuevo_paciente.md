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