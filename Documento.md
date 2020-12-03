### Visión general de la aplicación
* El resultado debe mostrar una captura semejante a esta pantalla siguiente:

<img src="Medios\2.PNG"/>

### Tarea 1.1: Crear y explorar el proyecto

* Este proyecto se creó en la práctica anterior, pero se definen sus características a continuación, para que se verifique que se cumplan cada uno de los requerimientos para lograr la práctica. Utilizando el conocimiento de creación de proyectos Android cree una App con las siguientes características:

* Ejecutar la aplicación creada y mostrar una captura del resultado

### Explorando el editor de diseño
* Brinde una breve reseña sobre las funcionalidades que presenta el editor de diseño, muestre una captura.

### Tarea 1.2: Agregar elementos Views en el editor de Layout

* Se crea el diseño de la interfaz de usuario para la aplicación HelloToast en el editor de diseño mediante las características ConstraintLayout. Puede crear las restricciones manualmente, como se muestra más adelante, o automáticamente mediante la herramienta Conexión automática.

### Examinar las restricciones (constraint) de los elementos
* Abra activity_main.xml desde el panel Proyecto > Android si aún no está abierto. Si la pestaña Design (diseño) aún no está seleccionada, haga clic en ella.

<img src="Medios\3.PNG"/>

* Si no hay ningún blueprint, haga clic en el botón Select design surface de la barra de herramientas (puede presionar la tecla B, para cambiar entre cada modo) y elija Design + blueprint

<img src="Medios\4.png"/>

* La herramienta Conexión automática también se encuentra en la barra de herramientas. Está habilitado de forma predeterminada. Para este paso, asegúrese de que la herramienta no está deshabilitada

<img src="Medios\5.PNG"/>

* Haga clic en el botón de acercar para acercar los paneles de diseño y blueprint para ver de cerca.

* Seleccione TextView en el panel del árbol de componentes (Component tree). El "Hello World" se resalta en los paneles de diseño y blueprint y las restricciones para el elemento TextView son visibles.

<img src="Medios\8.PNG"/>

* A continuación, se muestra como establecer una restricción o constraint con el contenedor padre al lado derecho del TextView

<img src="Medios\1.PNG"/>

Observe detenidamente el contorno del TextView, puede identificar un circulo al borde del elemento en cada uno de sus lados, estos sirven para establecer restricciones con sus elementos próximos. En cambio, los cuadrados en las esquinas si los arrastra hacia afuera del elemento puede cambiar el tamaño de este.

### Añadir un botón al layout

Cuando está habilitada, la herramienta Conexión automática crea automáticamente dos o más restricciones para un elemento de interfaz de usuario en el diseño primario. Después de arrastrar el elemento al diseño, crea restricciones basadas en la posición del elemento.

<img src="Medios\6.PNG"/>

## Siga estos pasos para agregar el Button:

* Comience con una pizarra limpia. El elemento TextView no es necesario, por lo que mientras está seleccionado, pulse la tecla Supr o elija Edición > Eliminar. Ahora tiene un diseño completamente en blanco.

<img src="Medios\1.PNG"/>
Acá tendriamos que eliminar dl botton de Hola wordl.

* Arrastre un botón desde el panel Paleta a cualquier posición de la presentación. Si coloca el elemento Button en el área media superior de la presentación, pueden aparecer restricciones automáticamente. Si no es así, puede arrastrar restricciones a la parte superior, izquierda y derecha del diseño

* Añada un segundo botón en la parte inferior del layout y del mismo modo cree las restricciones correspondientes con los elementos próximos a él.

* Pruebe borrar todos los constraints o restricciones de un elemento, seleccionando y pasando el puntero sobre este y seleccionar cleal all constraints

<img src="Medios\7.PNG"/>

### Tarea 1.3: Cambiar los atributos de los elementos de la interfaz de usuario

En esta tarea, ingresa nuevos valores y cambia los valores de los atributos importantes de Button, que son aplicables a la mayoría de los tipos de vista.

### Cambiar el tamaño del Button

* El editor de layout ofrece controles de cambio de tamaño en las cuatro esquinas de una view para que pueda cambiar el tamaño de la view rápidamente. Puede arrastrar los controladores en cada esquina de la View para cambiar su tamaño, pero al hacerlo, codifica las dimensiones de ancho y alto. Evite la codificación de tamaños para la mayoría de los elementos de Vista, porque las dimensiones codificadas no se pueden adaptar a diferentes tamaños de pantalla y contenido.

* En su lugar, use el panel Atributos en el lado derecho del editor de layout para seleccionar un modo de tamaño que no use dimensiones codificadas. El panel Atributos incluye un panel de tamaño cuadrado llamado inspector de vista en la parte superior. Los símbolos dentro del cuadrado representan la configuración de alto y ancho:

<img src="Medios\9.PNG"/>

* Height Control: Este control especifica el atributo layout_height y aparece en dos segmentos en los lados superior e inferior del cuadrado. Los ángulos indican que este control está configurado en wrap_content, lo que significa que la Vista se expandirá verticalmente según sea necesario para adaptarse a su contenido. El "8" indica un margen estándar establecido en 8 dp.

* Width Control: Este control especifica layout_width y aparece en dos segmentos en los lados izquierdo y derecho del cuadrado. Los ángulos indican que este control está configurado en wrap_content, lo que significa que la Vista se expandirá horizontalmente según sea necesario para adaptarse a su contenido, hasta un margen de 8 dp.

* Botón de cierre del panel atributos. Haga clic para cerrar el panel

### Siga los siguientes pasos:

* Seleccione el botón superior en el panel Árbol de componentes.

* Haga clic en la pestaña Atributos en el lado derecho de la ventana del editor de layout.

<img src="Medios\10.PNG"/>

* Haga clic en el control de ancho las veces que sea necesario; debe lograr el valor match_constraint para el layout_width

<img src="Medios\11.png"/>

* Realice la misma modificación para el botón inferior, el resultado es que ambos botones deben cubrir todo el ancho del constraint.

<img src="Medios\12.png"/>
