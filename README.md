# Paper-de-Arquitecturas

¿Para que usar arquitectura en un software?

La pregunta la podriamos re plantear diciendo ¿Para que programo?, cuando nuestro enfoque tiene previsto una mayor escalabilidad en lo que estamos desarrollando siempre es necesario desarrollar un buen patron de diseño y bases para que en ese futuro previsto tengamos la posibilidad de escalarlo sin inconvenientes y mas tiempo del que se necesitaria.

¿Por que se suele utilizar mas en equipos de trabajo?

Cuando hablamos de arquitecturas escalables siempre suele tener mas presencia en el campo laborar de manera “grupal”. Esto lo que permite es combinar todas las tarea con buenas metodologias y no tener que reinventar la rueda cuando otra persona de nuestro equipo ya soluciono algo parecido.

¿Cuanto es la tasa de exito en un proyecto profesional sin utilizar una arquitectura?

Hace 4 años la tasa era de un 40% notificado lo que de manera forzada fue moviendo el mercado y las capacitaciones internas de las empresas para empezar a emplear nuevos y mejores sistemas optimizados de desarrollo.

¿Por que hacemos ponemos como tan importante documentar todo?

Poniendo de ejemplo la lectura de un libro y el objetivo de aprenderlo de la manera mas optima posible, la mejor manera de hacerlo es viendo un resumen donde se mencionen los temas principales del mismo.

Esto mismo se aplica en el desarrollo cuando documentamos el funcionamiento de un proyecto y la manera de hacer un deploy.

¿Que problemas evita implementar esto en un equipo de desarrollo?

Si bien anteriormente se menciono el tema que tiene muchas presencia en la escalabilidad y futuro del proyecto. Tambien sirve muchisimo para evitar re desarrollo de un “modulo” por mala comprension desde un principio…

Cuando un proyecto se realiza sobre bases solidas como por ejemplo:
1- documentacion

2- diagrama de flujo independiente de cada micro-servicio (servidor)

3- conexion del ese mismo diagrama con el diagrama del (cliente)

En resumen cuando previamente se establecen unas buenas bases en el proyecto se puede evitar problemas muy comunes en un gran promedio de empresas.

Hablando enfocado en tema modular.. ¿Por que se suele recomendar tanto el singleton?

Actualmente se utiliza mucho esta metodologia hablando en el codigo del proyecto ya que evita muchisimos dolores de cabeza cuando cada modulo es independiente del otro.

Por ejemplo cuando hablamos de soluciones.. los microservicios lo que solucionan es esto mismo, modularizar el proyecto al maximo para que cada minima funcion este atomicamente realizada.

Si bien es muy probable que es mas de una situacion nos encontremos que es imposible realizar esto cuando un servicio/metodo/componente requiere forzadamente dependencia de otra. A lo que nos referimos con esto es que si bien puede ser dependiente no debe serlo estrictamente para correcto funcionamiento de la aplicacion.

¿Cual es el rol del arquitecto del software?

En simples palabras es proponer, mantener y diseñar la arquitectura del proyecto. Esto teniendo en cuenta los datos del proyecto.

Casos de uso

Posible crecimiento

Pruebas de riesgos mas probables  /subItem 1*

Datos etc.

Se suele hacer un analisis previo para busca un equilibrio entre diseño/requirements, ya que es inutil hacer la arquitectura que tiene “facebook” para una aplicacion a nivel local. no es optimo en proporciones de plata,tiempo etc.

SUBITEM 1:  El planteo de los riesgos se debe contemplar a la par de un tester donde se le indica desde un principio los problemas que puede surgir y en cada prueba se contempla las mismas bases iniciales.

¿Por que en muchas empresas el arquitecto de software no existe y el trabajo lo realiza en equipo en conjunto?

Napoleon dijo: “Si quieres que algo salga adelante encargaselo a una persona, si quieres que parezca que quieres que salga adelante propone un comite”.

¿Cual es modelo o digrama minimo para considerarse una arquitectura y no un patron?

El modelo de vista arquitectonica 4+1  es un metodo muy utilizado. Las cuatro vistas son la vista logica, la vista de desarorollo, la vista de proceso y la vista fisica. 

La vista logica: se centra en la funcionalidad expuesta a los usuarios finales

La vista de desarrollo: muestra como esta estructurado el sistema, haciendo hincapie en la preocupaciones de los desarrolladores y testers.

La vista del proceso: muestra el aspecto dinamico del sistema y como se comporta durante la ejecucion.

La vista fisica muestra como esta dispuesto o distribuido el sistema y como se conectan los componentes entre si.

El “+1” se refiere a los escenarios, que muestran casos de uso del sistema y proporcionan un contecto para entender las anteriores vistas.
