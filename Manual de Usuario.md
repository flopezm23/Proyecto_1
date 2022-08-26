# Programa de soporte para control de tickets, OPEN SOURCE TICKET REQUEST SYSTEM (OTRS)

Este programa ha sido creado para facilitar el manejo y control de casos o tickets de una agencia de resolución de problemas que está organizada en varios departamentos.

# Derechos de autor

Este programa fue realizado por *Fernando Omar López Morales con numero de carné: 7690-21-20755* de la facultad de Ingeniería de la Universidad Mariano Gálvez, sede Boca del Monte del departamento de Guatemala, con fecha de 23/08/2022

## Sobre Agencias de resolución de problemas y atención al cliente

Un centro de soporte es el punto de contacto en el cual se solucionan los problemas que surgen entre los usuarios o clientes de un proveedor de servicios.

Generalmente un centro de soporte utiliza un sistema de manejo de información basado en "tickets", que es administrado por los departamentos de soporte general así como los departamentos de soporte avanzado.
## Componentes del Centro de resolución de problemas
- Tickets
Conjunto de información importante sobre un caso, clasificada estratégicamente para que el ticket pueda ser trabajado.
- Departamentos
La organización está dividida en departamentos que cuentan con habilidades y capacitación diferente para la resolución de problemas.
Los departamentos están organizados por responsabilidades mas también de una forma jerárquica, siendo el departamento de desarrolladores el nivel más alto.
- Bitácora
Es un informe detallado del recorrido de un ticket desde su ingreso al sistema hasta su resolución definitiva en cualquiera de los departamentos asignados.
# Tickets
**Características de los tickets**
Todos los tickets son un conjunto de información en donde se especifica el usuario afectado y el problema, entre las informaciones más importantes de un ticket encontramos las siguientes:
- Nit del usuario: identificación del usuario que está experimentando el problema.
- Problema: Inconveniente que ha sido reportado al soporte.
- Estado: Identificación del proceso de resolución del ticket, si el ticket aún no es resuelto mantendrá el estado de "Activo".
- Cola o departamento asignado: Al igual que el estado, Cola es un identificador del ticket que demuestra en cuál departamento a sido asignado para su resolución.
## Estados de un ticket
**Activo**
Un ticket se encuentra en estado de activo mientras este aún no haya sido resuelto.
**Resuelto**
Cuando un caso es resuelto el estado del ticket cambia de "Activo" para "Resuelto".

## Departamentos
**Mesa**
Este es el departamento general en donde todos los tickets o casos son ingresados, los empleados de este departamento cuentan con una capacitación básica de resolución de problemas, y se pretende que los empleados de este departamentos sean capaces de resolver todos los problemas simples que llegan al sistema, sin embargo, en caso de que un problema no haya sido resuelto, tienen autorización de escalar un ticket para el departamento de Soporte.
Este departamento la prioridad se determina por el sistema **FIFO** (Primero en Entrar es el Primero en Salir).
**Soporte**
A diferencia del departamento Mesa, los integrantes del departamento de Soporte cuentan con una capacitación más completa y se espera que sean capaces de resolver la mayoría de tickets que reciben ya sea transferencia de la Cola Mesa, o tickets que ingresan directamente hacía ellos. 
Así como en la Cola Mesa, si un problema no logra ser resuelto, los empleados de este departamento aún pueden escalar el caso para el departamento de "Desarrolladores".
**Desarrolladores**
Este es el departamento más capacitado y encargado de proveer una respuesta a todos los casos, la opción de escalar ya no está disponible para este departamento.
Los tickets asignados a este departamento o Cola, pueden venir desde el ingreso de nuevos tickets o de tickets escalados por el departamento de Soporte.
## Bitácora

El programa puede ser ejecutado desde el entorno de NetBeans desde cualquier computador que cuente con esta aplicación.

## Manipulación del programa
Al ejecutar el programa este muestra en el menú todas las opciones disponibles las cuales se dividen en tres secciones:
- Manipulación de informaciones de los clientes
- Manipulación de informaciones de los productos
- Manipulación de algunas informaciones de las facturas existentes 
## Interacción de empleados del soporte
Todos los empleados deben identificarse al ingresar al programa, entre las informaciones requeridas se encuentra su número de Nit y también su rol o departamento al que pertenece.

Después de que un empleado se identifica el programa reconoce la función de este empleado y el departamento al que pertenece.

Todos los tickets se encuentran almacenados en el sistema y por lo tanto cuando el sistema logra identificar los tickets que pueden ser trabajados por este empleado, toma el ticket según la prioridad del departamento y se lo asigna o presenta al empleado para que pueda trabajarlo.
## Funciones adicionales
**Agregar ticket**
Cada vez que un nuevo ticket es agregado al sistema este es clasificado según la Cola, y todos los nuevos ticket ingresan con el estado de "Activo". 
Para agregar un ticket al sistema es necesario que este cuente con algunas informaciones importantes:
- Nit del usuario.
- Id del usuario (en números enteros).
- Problema: descripción clara sobre el inconveniente del cual se espera una resolución.
- Cola: departamento al que el ticket desea ser entregado.

**Resolver ticket**
Al resolver un ticket independientemente del departamento en donde haya sido trabajado, es necesario registrar a través de un mensaje la resolución de dicho problema; en otras palabras, el empleado explica como se resolvió el problema, y el sistema cambia el estado del ticket de "Activo" a "Resuelto".
**Escalar ticket**
Cualquier ticket que se encuentre en la cola de Mesa o de Soporte pueden ser escalados para uno de los departamentos avanzados desde su posición, un departamento a la vez.
**Registros de la Bitácora**
Cada vez que sucede algo en uno de los tickets, este evento es registrado en la Bitácora, identificando el ticket que sufrió el evento y así mismo la acción que se llevó acabo.
**Reporte 1**
El Reporte 1 presenta todos los tickets del sistema independientemente del estado en el que se encuentran y la Bitácora.
**Reporte 2**
El Reporte 2 presenta los tickets organizados por Colas.
**Reporte 3**
El Reporte 3 presenta cada uno de los tickets con su respectivo registro en la Bitácora, identificando ambos por el Nit del usuario.
# Lenguaje de programación utilizado

Esta aplicación fue creada en el lenguaje Java, utilizando especialmente el IDE de Intelli JIDEA Community Edition 2022.1.3.
## Material de apoyo
cognizant. Centro de soporte. Sitio Web:
https://www.cognizant.com/es/es/glossary/service-desk
## Video con explicación del programa: https://youtu.be/P25ixmk3QTY

