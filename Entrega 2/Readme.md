# Letra entrega 2 - Semestre 2, 2019

En esta entrega ya empezarás a ver como aparecen elementos que pueden ser relacionados a tu proyecto final. Para ello, vamos a acotar el problema a algo simplificado y general a todos, creando un simulador de mundos muy simple.

## Parte 1 - Modelado de mundo
Como primer paso, deberás modelar y programar un mundo, el cual contendrá uno o más niveles de dos dimensiones. 
Estos niveles se corresponderán con una grilla, donde en cada celda del nivel podrá haber un único elemento. 
Estos elementos podran ser:
 * Botones
 * Imagenes
 * Elementos que se pueden arrastrar y soltar 

No será necesario en esta primer instancia agregar comportamiento a los elementos, simplemente poder representarlos en pantalla de forma estática. Sin embargo, si te animas a agregar más, adelante!

**Recomendación!** Antes de empezar a escribir código, modela tu solución de forma gráfica con tarjetas CRC o un diagrama de clases sencillo. De todas maneras deberas hacer esto para la entrega, así que puedes hacerlo como primer paso.

## Parte 2 - Simulación gráfica
Para poder realizar esta simulación, es importante contar con alguna forma de representar gráficamente este mundo. 
Para que no pierdas tiempo estudiando cómo dibujar en pantalla estos elementos, te proveemos de una biblioteca que resuelve esto por ti, a la cual accedes en: 
https://github.com/ucudal/PII_Proyecto2019

## Parte 3 - Persistencia de modelo
Ya que has aprendido a crear objetos a partir de un archivo plano, podrás aprovechar esta nueva habilidad para crear un mundo a partir de un archivo también. Esto significa que tu mundo puede ser construido y alterado simplemente modificando un archivo de texto!
Para ello, deberás definir diferentes tags y qué tipo de objetos serán creados según el tag. Esto puede parecer un problema complejo, pero seguramente alguien ya pasó por esto e inventó algúna solución. Podríamos hasta suponer que esto es un problema recurrente. Un patrón que se repite tal vez... :wink:

### Ejemplo:
A modo de ejemplo, supongamos que tenemos el siguiente archivo de entrada:

```HTML
<square-world size="50" name="world1">
	<level name="level1" world="world1">
		<button name="button1" level="level1" position_x="10" position_y="20" size="20x30">
	</level>
</square-world>
```
Podriamos a partir de este archivo crear un mundo cuadrado de 50x50, el cual contiene un nivel llamado "level1" y dentro de ese nivel un único botón de tamaño 20x30 ubicado en la posición (x=10,y=20) del nivel. 

**Ten en cuenta que esto es solamente un ejemplo y no necesariamente debas modelar tu solución de esta forma!**

## Parte 3 - Documentación
Deberás entregar, además de tu código, un diagrama de clases sencillo utilizando UML (tal como los vistos en clase) 
En estas representaciones gráficas solamente es necesario referenciar a las clases que has diseñado tu y las colaboraciones que utilices. 

## Entrega
La entrega deberá ser en Github y Webasignatura. Para ello, deberás subir a webasignatura la URL del commit que quieras que sea evaluado. Si la fecha y hora del commit indicado es posterior a la fecha y hora de la entrega, se evaluará el último commit antes de la fecha de corte. La consigna es la misma para todos y cumplir con las restricciones de tiempo es importante para la vida de estudiante así como para la vida profesional a futuro.

#### Importante
Recuerda que un programa debe incluir casos de prueba en xUnit y documentación docFX. 
Los casos de prueba deben asegurarse de que cada método de cada clase que programaste funcione como es debido. Intenta utilizar esto como una herramienta para trabajar menos y más seguro, y no como un requisito “burocrático”.

#### Reglas de colaboración
Los ejercicios son en equipo. Puedes diseñar una solución en conjunto con tus compañeros de equipo u otros equipos y aprovechar comentarios o correcciones de los profesores, pero todos los integrantes del equipo deben poder comprender y replicar el código entregado, compilarlo y ejecutarlo, así como las decisiones de diseño utilizadas para generar el mismo. 

#### Entregas por correo electrónico
No se aceptarán entregas por correo electrónico excepto que Web Asignatura y Github no estén disponible seis horas antes a la fecha final de entrega. La entrega por correo eletctrónico debe enviarse a todos los profesores y pedirles confirmación de entrega. Es tu responsabilidad asegurarte de que el trabajo haya sido recibido.
