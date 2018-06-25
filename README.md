# CARON
**Fase Inicial**

**Nombre del proyecto:** _Aplicativo para la gestión de visitas en establecimientos carcelarios_

**Problemática que resuelve :**

Las visitas que se dan durante sábados y domingos dentro de los centros de reclusión consisten en un procedimiento extenso, tedioso y sin organización. Para solicitar la cita que permite a miles de mujeres y hombres ver a un familiar que está recluido se vive todo un viacrucis, las personas deben estar desde las 4 o 5 AM esperando la llegada a un primer filtro, posteriormente se les solicita el registro donde otro empleado solicita una foto de medio cuerpo, la cédula de ciudadanía y una fotocopia de la misma. Nada más este proceso ya ha tomado un tiempo considerable.

Luego, vienen procesos de asignación de identificadores que se hace de una manera muy &quot;rústica&quot; , pues se escribe en el brazo de la persona el número, la siguiente estación , es la estación más importante pues en esta se imprime un ticket que contiene información como: nombre del interno, patio en el que se encuentra, nombre del visitante, parentesco con el recluso y número de turno. Finalmente vienen las estaciones de requisa de visitantes y los elementos que se piensan ingresar a la cárcel.

Este procedimiento dura alrededor de 1 hora por persona, si todo sale bien y no hay problemas con la información del visitante y los objetos que porta. No obstante, los inconvenientes en registro y requisas son más comunes de lo que parecen, es por eso que ese tiempo puede variar considerablemente y ralentizar el procedimiento de otros visitantes. De igual forma , los registros de visitas no se consignan de forma correcta y esta información que es importante para el establecimiento penitenciario no se obtiene de manera oportuna. Se observa entonces, que el problema central para visitas en los centros de reclusión es el tiempo que se pierde en filtros demandantes que podrían disminuir con ayuda de un sistema que reúna la información previamente.

**Definición del proyecto:**

El proyecto de software consiste en un aplicativo web orientado a facilitar y agilizar el proceso de agendamiento de citas de visita a los reclusos de los centros penitenciarios de la capital. Dentro de este aplicativo se deben mantener todos los datos relacionados con los reclusos, los empleados del INPEC y los visitantes, esto con el fin de corroborar la información de cada actor a la hora de agendar una visita.

El proyecto cuenta con 5 módulos principales:

1. **Registro de usuarios:** Destinado al registro de información básica de cada actor del sistema (visitante, empleado centro carcelario y recluso), el visitante y el empleado deberán registrarse en el sistema manualmente, mientras que los empleados registran a los reclusos de los cuales son responsables.
2. **Solicitud de visita:** Módulo encargado de solicitar una visita al sistema, el visitante deberá proveer información adicional a la hora de solicitar una visita, tales como el parentesco, documento de identificación, motivo de la visita, ingreso de elementos al centro carcelario con destino al recluso y etc. La solicitud luego se le remite al empleado a cargo del recluso que se va a visitar.
3. **Verificación de requerimientos del visitante:** Una vez remitida la solicitud de la visita, el empleado del centro carcelario se encargará de verificar y validar la información anexada por el visitante, así mismo verificará la condición del recluso, tales como su estado (disponible, aislado, hospitalizado, fuera del centro carcelario), la voluntad de asistir a la visita y en caso de que se vayan a ingresar elementos, verificar que cumplen con las normas del centro carcelario.
4. **Agendamiento de citas:** Finalmente dependiendo del resultado del módulo anterior, se verificará la disponibilidad de citas en el calendario del centro carcelario y se le agendará una cita, la cual se le notificará por medio de una notificación en el aplicativo y un correo electrónico que informará el resultado de la solicitud, si ésta no es aprobada, se le informará los requerimientos que no cumplió y si es aprobada se le informará el día, la hora, el lugar, la sala de visita, y las recomendaciones a seguir al momento de la visita, así mismo se le enviará una etiqueta en formato PDF con código de barras y la información del visitante y el recluso que va a visitar que deberá imprimir y portar el día de la visita.
5. **Histórico de visitas:** El día en el que se lleva a cabo la visita el empleado del INPEC deberá registrar la asistencia del visitante al centro carcelario, así mismo se detallará información como la hora de inicio y fin de la visita, los elementos confiscados y otros detalles adicionales que se presenten durante la visita. Este histórico lo podrán consultar tanto los visitantes como los empleados del centro carcelario siempre que quieran, los visitantes podrán consultar el registro de ellos mismos, mientras que los empleados sólo podrán revisar los registros de los reclusos que tienen a cargo.



**Objetivos:**

**General:**

Entregar un prototipo de plataforma para la gestión de las visitas carcelarias partiendo de la obligación de orden, facilidad y accesibilidad de los establecimientos carcelarios, teniendo una visión sistémica de las necesidades de los reclusos, sus cercanos y los empleados encargados de diligenciar todo el proceso de planificación, realización y evaluación de las visitas, con el fin de brindar un sistema que cumpla con las exigencias legales hacias sus involucrados.

**Especificos:**

- Apoyar la planificación de la oferta de cupos de visita y sus locaciones.
- Mantener y recuperar la información de los reclusos (con su ubicación en el centro penitenciario), de sus visitantes y de los encargados de controlar la visita.
- Verificar la información entregada por un visitante al momento de su registro.
- Habilitar un canal de fácil acceso para la solicitud y agendamiento de la visita carcelaria.
- Reducir el protocolo y las formalidades al momento de registrar y acceder a la información de una visita penitenciaria.
- Controlar el registro e ingreso de elementos al centro penitenciario, facilitando la trazabilidad entre lo descrito y lo portado.
- Ofrecer acceso a datos históricos de las visitas realizadas para apoyar futuras tomas de decisiones.

**Alcances y Limitaciones**

**Alcances**

La plataforma tendrá un registro de tres tipos de usuarios: los administrativos, los reclusos y los visitantes. Los administrativos tienen la función de gestionar la información de los reclusos, tal como datos personales, fecha de ingreso, fecha de salida, celda, sanciones, delitos y un identificador; así mismo, los administrativos se encargan de gestionar la información asociada a los visitantes, ya que cada visitante requiere una validación por parte de los administrativos para acceder como visitante, por lo tanto un administrativo es quien permite o niega una solicitud de visita. Además, el rol de los administrativos es cumplido por los diferentes empleados de la organización, que tengan los permisos para llevar a cabo estas funciones; por lo tanto, los empleados encargados también son registrados dentro del sistema con su información personal, identificadores y función. Los reclusos son únicamente registrados por los administrativos.

El rol de visitante lo cumplen aquellos familiares o cercanos de algún recluso, que quiera ir de visita. En este caso, el visitante debe cumplir dos pasos: el primero, hacer un registro en la plataforma con su información personal, además de adjuntar una copia de la cédula de ciudadanía; el segundo, solicitar un agendamiento de cita donde se debe especificar el recluso a quien va a visitar, la fecha, la hora, el parentesco, el motivo de visita, los ítems que va a aportar, en caso que los haya, además de sustentar la información al adjuntar los siguientes documentos: una constancia de parentesco, un compromiso firmado no mayor a tres meses de antigüedad, una foto a color de medio cuerpo reciente, y para los visitantes menores de edad, un extrajuicio notarial de aprobación de la visita por sus representantes. La asignación de la visita no será aprobada en caso de que el recluso tenga una sanción u otros factores que limitan al recluso o al mismo visitante.

**Limitaciones**

- Según las reglas establecidas por el INPEC, para aprobar una solicitud de visita el funcionario encargado debe hacer la revisión de los documentos, además de cumplir con una visita domiciliaria; sin embargo, para este proyecto solo se tendrá en cuenta una suposición de los documentos requeridos, sin tener en cuenta la visita domiciliaria.
- El INPEC plantea que las instalaciones de las penitenciarías contienen más o menos 6000 reclusos; sin embargo, para las pruebas del proyecto no se tomará esa cantidad de datos sino una cantidad representativa.
- Las visitas solo se pueden llevar a cabo los sábados y domingos.
- El proyecto será orientado únicamente a las instituciones penitenciarias de Bogotá.
- El tipo de ítems que se pueden ingresar en la visita, será el acordado por INPEC en la resolución 6305de 20091.



**Criterios de Exito**

1. La información disponible debe ser encontrada fácilmente y estar disponible para los stakeholder del proyecto según sus necesidades.
2. La plataforma debe adaptarse a la legislación vigente de la región donde sea vaya a desplegada.
3. Se debe poder delimitar los derechos de acceso al control y cambio de la información de la plataforma.
4. La plataforma debe ser amigable, intuitiva y de navegación ágil.
5. Se debe cumplir con los tres criterios mínimos de seguridad.
 a. Autenticidad
 b. Confidencialidad
 c. Integridad
6. La plataforma debe proveer la posibilidad de generar un informe histórico para los diferentes criterios.
7. La información debe ser actualizable en tiempo real, con el fin de mantener las reglas del negocio.
8. Cada vez que quiera registrar una visita debe autenticarse los datos suministrados del visitante ante un ente externo.
9. La infraestructura tecnológica debe contar un sistema de duplicación de respaldo ante cualquier fallo.
10. La infraestructura tecnológica debe ser externa al ente penitenciario y debe garantizar su continuo funcionamiento.
11. La administración de la plataforma debe contar con la posibilidad de  acceso remoto.
12. La plataforma debe poder migrar la información desde documentos de archivo planos.

**Listado de tareas y construcción**

1. Hacer estudio de normas vigentes para la visita a reclusos
2. Analizar los requerimientos según por roles
3. Detectar falencias en los procesos del sistema
4. Delimitar la información relevante de los distintos roles
5. Construcción del componente de registro de usuarios
6. Construcción del componente de solicitud de visita
7. Construcción del componente de verificación de requerimientos del visitante
8. Construcción del componente del agendamiento de citas
9. Construcción del componente del histórico de citas
10. Migración de la información al sistema de información
11. Determinar mecanismos de autenticación de la información suministrada por los visitantes
12. Determinar mecanismos de confidencialidad para el manejo de la información
13. Delimitar los permisos de lectura y escritura por parte de los roles
14. Prueba del componente de registro de usuarios
15. Prueba del componente de solicitud de visita
16. Prueba del componente de verificación de requerimientos del visitante
17. Prueba del componente del agendamiento de citas
18. Prueba del componente del histórico de citas
19. Despliegue de la plataforma
20. Capacitación de los usuarios (empleados)
21. Socialización de la herramienta con la comunidad

**Propuesta estructura orgánica:**

![](/images/estructura_organica.png)

**Estimaciones**

![](/images/estimacionCostos.PNG)

![](/images/estimacionTiempos.PNG)

**Cronograma**

![](/images/cro1.PNG)
![](/images/cro2.PNG)
![](/images/cro3.PNG)
![](/images/cro4.PNG)
![](/images/cro5.PNG)
![](/images/cro6.PNG)
![](/images/cro7.PNG)
![](/images/cro8.PNG)
![](/images/cro9.PNG)
![](/images/cro10.PNG)
