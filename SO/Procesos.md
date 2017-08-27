# Procesos

Un proceso es un programa en ejecición, que incluye el código del programa y los recursos que consume, tales como la memoria, archivos, sockets, dispositivos, librerías, etc.

  * Código 
  * Datos
  * Stack. Cada item del stack representa una función
    * Parámetros
    * Variables locales
    * Lugar de retorno
  * Heap. Memoria asignada dinámicamente.

Un proceso en ejecución puede cambiar de estado

  * New
  * Running
  * Waiting
  * Ready
  * Terminated

Cómo sé el estado de mi proceso? Desde un terminal ejecutando `htop`, `top` o `ps aux`. La otra opción es usar un administrador de Procesos.

La estructua que representa un proceso para el SO se llama **Process Control Block (PCB)** consiste en una lista de punteros.
  * Estado
  * PID
  * PC
  * Registros de la CPU: *estado de la ejecución*
  * Información de *scheduling*
  * Información de memoria: límites, tablas de pñagina
  * Contabilidad
  * Información de I/O 

El cambio de proceso se conoce como **Context Switch**, consiste en guardar el estado del proceso que se va, cargar el estado del proceso qeu entra.

Un proceso crea a otro proceso pero cuál es el primero? Existe un porceso llamdo `init`, construido durante la inicialización del **kernel**. PID = 1.