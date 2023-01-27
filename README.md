# so1_actividades_201612132
Repositorio de la Actividad 1 del curso sistemas operativos 1

# 


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

