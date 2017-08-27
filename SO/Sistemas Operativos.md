## ¿ Para qué es un sistema operativo ?

El sistema operativo es el encargado de controlar que programa se ejecuta y cuando se lee los dispositivos I/O, entre otras tareas.

El sistema operativo **es** software que se **comunica** con el hardware. 

Existen dos modos para la CPU, *user mode* y *kernel mode* y el SO es el único programa que puede funcionar en kernel mode.

## Qué hace el sistema operativo?

Para el usuario: permite **usar efectivamente** el computador. Ejecutar programas, leer archivos, efectuar cálculos de manera limpia, fácil y ordenada.

Para el sistema computacional: permite **administrar los recursos**. Perminte multiplexar el uso de los recursos entre múltiples programas para eso se *virtualizan los recursos* de CPU, memoria y disco.

## De qué tamaño es un SO?

Esta compuesto por un kernel y programas del sistema.

  * Kernel: Un programa que permite controlar directamente el hardware. Provee funcionalidad mínima: acceso a CPU, memoria y dispositivos.
  * Programas del sistema: Extienden las funciones del kernel.

  ## Tareas de un SO

  * Administración de procesos
    * Proceso
    * Tablas (árbol) de procesos 
    * Comunicación entre procesos
  * Administración de memoria
    * Espacio de direcciones
    * Memoria Vurtual
  * Administración de almacenamiento
    * Archivos
    * Directorios
    * Rutas absolutas y relativas
  
  ## Cómo funciona el SO?

  Los sitemas operativos son manejados por **interrupciones** y **traps**. El SO debe controlar que los procesos no puedad acceder a datos al que no tengan permiso, que no puedan monopolizar el uso de la cpu y que no puedan alterar el funcionamiento de otro proceso.

  Solo el SO debe ser capaz de administrar el *hardware*, y no los procesos.

## System Calls

Los programas utilizan llamadas al sistema frecuentemente