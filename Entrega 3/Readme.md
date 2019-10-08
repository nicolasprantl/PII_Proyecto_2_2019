# Universidad Católica del Uruguay
<img src="https://ucu.edu.uy/sites/all/themes/univer/logo.png"> 

## Facultad de Ingeniería y Tecnologías
### Programación II - Proyecto

# Letra entrega 3 - Semestre 2, 2019
![readme](../img/readme.jpeg?raw=true)

## Parte 1 - Motor del juego
Si has llegado a este punto del proyecto, has podido crear un modelo estático de tu juego a partir de un archivo con tags creados por ti. Pero, ningún juego es estático! Debemos agregarle comportamiento para que nuestro juego tenga algo de gracia.

Para ello, te pedimos que en este momento agregues a tu juego un motor de lógica. Este motor será quien contenga todas las reglas de tu juego. Deberá poder modificar el estado de tu modelo de acuerdo a las acciones realizadas, concer en todo momento el estado del juego (puntos, ganadores, perdedores), etc.

Actualmente tu proyecto deberia verse de la siguiente forma:
</br>

![AsIS](../img/as_is_motor.png?raw=true)
</br>
Donde Unity invoca al método Build, pasando un IMainviewAdapter. Dentro de este mótodo se ejecuta el/los métodos necesarios para generar un modelo en memoria a partir del XML y luego se le indica a Unity, a través de el IMainViewAdapter cómo representar este modelo en pantalla.

Luego de los cambios de esta entrega, tu sistema debería verse de la siguiente forma:
</br>

![ToBe](../img/to_be_motor.png?raw=true)
</br>
En este nuevo escenario, tu **motor** será quien interactue con Unity y deberá asegurarse de mantener actualizados los cambios en el **modelo** para reflejar los cambios en la interfaz de usuario realizados a través de Unity.

## Parte 2 - Testea el motor
Para esta entrega, no te vamos a dar una libreria de unity actualizada que permita simular todo el comportamiento. Por lo tanto, deberás crear un proyecto de test capaz de verificar que tu motor de juego se comporta correctamente. No solamente deberás verificar que el motor funciona bien, tambien deberas corroborar que el modelo es alterado de forma adecuada ante cada acción simulada.

El siguiente diagrama resume como estos componentes deberán interactuar entre si. En este caso verás que Unity no es parte del diagrama, ya que tus tests deberían funcionar y verificar que el motor y Modelo hacen lo que corresponde sin importar el framework de GUI.
</br>

![Testing](../img/testing.png?raw=true)
</br>

## Parte 3 - Documentación
Deberás extender el diagrama de clases creado para la entrega anterior, agregando las nuevas clases  de esta entrega. Al igual que en la entrega anterior, no es necesario utilizar ninguna herramienta para hacer los diagramas. Lápiz y papel es más que suficiente.
Recuerda que solamente es necesario referenciar a las clases que has diseñado tu y las colaboraciones que utilices. 

## Parte 4 - Style!
Para esta entrega ya vamos a ser más exigentes con las reglas de estilo de código. Te recomendamos por lo tanto, dejar de ignorar StyleCope (o comenzar a usarlo si no lo haces aún). Intenta que tu código tenga la menor cantidad de warnings de StyleCop posibles (lease cero!). 

## Entrega
La entrega deberá ser en Github y Webasignatura. Para ello, deberás subir a webasignatura la URL del commit que quieras que sea evaluado. Si la fecha y hora del commit indicado es posterior a la fecha y hora de la entrega, se evaluará el último commit antes de la fecha de corte. La consigna es la misma para todos y cumplir con las restricciones de tiempo es importante para la vida de estudiante así como para la vida profesional a futuro.

#### Importante
Recuerda que un programa debe incluir casos de prueba en xUnit y documentación docFX. 
Los casos de prueba deben asegurarse de que cada método de cada clase que programaste funcione como es debido. Intenta utilizar esto como una herramienta para trabajar menos y más seguro, y no como un requisito “burocrático”.

#### Reglas de colaboración
Los ejercicios son en equipo. Puedes diseñar una solución en conjunto con tus compañeros de equipo u otros equipos y aprovechar comentarios o correcciones de los profesores, pero todos los integrantes del equipo deben poder comprender y replicar el código entregado, compilarlo y ejecutarlo, así como las decisiones de diseño utilizadas para generar el mismo. 

#### Entregas por correo electrónico
No se aceptarán entregas por correo electrónico excepto que Web Asignatura y Github no estén disponible seis horas antes a la fecha final de entrega. La entrega por correo eletctrónico debe enviarse a todos los profesores y pedirles confirmación de entrega. Es tu responsabilidad asegurarte de que el trabajo haya sido recibido.
