# so1_actividades_201612132
Repositorio de la Actividad 1 del curso sistemas operativos 1

# Tipos de kernel y sus diferencias

* **Monolítico:**  
Este tipo de kernel tiene una estructura única donde todos los subsistemas se encuentran en un único módulo lógico. Carece de unas interfaces bien definidas entre subsistemas y permite trabajar en un solo espacio de direcciones cuando se carga el código en la memoria RAM, lo que reduce la complejidad. Además, trabajará en su totalidad en modo supervisor. Algunos ejemplos de sistemas con kernel monolítico son DOS, MacOS, OpenVMS, Multics, otros Unix, y Linux.

* **Microkernel:**
Es un micronúcleo que tiene una estructura modular, es decir, los subsistemas no se encuentran en un único módulo lógico, sino que cada uno está en un módulo propio. Esto hace que resulten más fáciles de desarrollar, pero su rendimiento puede ser inferior.

* **Híbrido:**
Es una mezcla de los dos conceptos anteriores, con una estructura básica como un microkernel y otras partes de código no esenciales como módulos. 

* **Nanokernel:**
Este tipo de kernel es muy recudido, aún más pequeño que un microkernel. Son usados para sistemas embebidos porque aporta mucha fiabilidad.

* **Exokernel:**
Está estructurado de forma vertical, con una estructura bastante novedosa. Son núcleos pequeños y se crearon con fines de investigación. En este caso, los programas son los encargados de tomar decisiones sobre la gestión de recursos de hardware haciendo uso de ciertas bibliotecas.




# User vs Kernel Mode

| Modo Kernel   | Modo Usuario |
| ------------- | ------------- |
| En modo kernel, el programa tiene acceso directo y sin restricciones a los recursos del sistema. | En modo usuario, el programa de aplicación se ejecuta y se inicia. |
| En el modo Kernel, todo el sistema operativo puede dejar de funcionar si se produce una interrupción   | En el modo de usuario, un solo proceso falla si ocurre una interrupción.     |
| 	El modo kernel también se conoce como modo maestro, modo privilegiado o modo de sistema.  | El modo de usuario también se conoce como modo sin privilegios, modo restringido o modo esclavo.  |
| Todos los procesos comparten un único espacio de direcciones virtuales.  |   Todos los procesos obtienen un espacio de direcciones virtuales separado. |
|  Las aplicaciones tienen más privilegios que en el modo usuario. | Las aplicaciones tienen menos privilegios. |
| Puede acceder tanto a los programas del usuario como a los programas del kernel, no hay restricciones.  | Necesita acceder a los programas del kernel, ya que no puede acceder a ellos directamente.  |
| El bit de modo de kernel-mode es 0.  | Tiempo; el bit de modo del modo de usuario es 1. |

