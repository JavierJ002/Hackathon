![image](https://github.com/user-attachments/assets/617d4b19-4fa0-4ba6-9a80-181a179171fe)
                          Sistema de seguridad tradicional, basado en DAC(Acceso de discrección del usuario)

La idea de este sistema es que el usuario utiliza un conjunto de permisos y puede acceder al contenido y maniipularlo en base a ellos.
El problema de esto, es que un usuario tiene acceso a múltiples sistemas (contextos) de la aplicación que pueden comprometer al sistema
en caso de intrusión. 

La idea de SELinux es crear una capa extra de seguridad donde se utiliza una metodología de MAC (Mandatory Access Control), donde 
cada función está segregada dependiendo de su contexto. Este contexto esta representado por las etiquetas que se le den a cada servicio.
La idea es que cada servicio, sea un dominio y cada proceso puede acceder a cada función dependiendo de su contexto, con la idea de minimizar
un daño en caso de que haya una intrusión.

![image](https://github.com/user-attachments/assets/aa2eee3c-82ff-4db9-b095-0fcc95f7fb18)



Comandos Clave para entender, manipular y capturar la esencia de SELinux:


Archivos Binarios o Logs: Ellos nos permiten conocer el dominio de cada servicio. Se puede averiguar la ubicación mediante el comando which + servicio


![image](https://github.com/user-attachments/assets/0fb2cf2a-3d85-4b4d-bdc9-06fcf619fcb6)
