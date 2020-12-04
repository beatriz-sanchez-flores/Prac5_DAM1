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

<img src="Medios\13.PNG"/>

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

<img src="Medios\14.png"/>

* Haga clic en la pestaña Atributos en el lado derecho de la ventana del editor de layout.

<img src="Medios\10.PNG"/>

* Haga clic en el control de ancho las veces que sea necesario; debe lograr el valor match_constraint para el layout_width

<img src="Medios\11.png"/>

* Realice la misma modificación para el botón inferior, el resultado es que ambos botones deben cubrir todo el ancho del constraint.

<img src="Medios\12.png"/>

<img src="Medios\15.PNG"/>

* Establezca wrap_content al layout_height, también puede usar un valor fijo de 16dp

<img src="Medios\16.PNG"/>

### Cambiar los atributos de Button

* Para identificar cada vista de forma única dentro de un diseño de actividad, cada vista o subclase de vista (como el botón) necesita una identificación única (id). Y para ser de alguna utilidad, los elementos del botón necesitan texto. Los elementos de vista también pueden tener fondos que pueden ser colores o imágenes.

* El panel Atributos ofrece acceso a todos los atributos que puede asignar a un elemento de Vista. Puede ingresar valores para cada atributo, como los atributos android:id, background, textColor y text.

### Siga los siguientes pasos:

* Después de seleccionar el primer botón, edite el campo ID en la parte superior del panel Atributos a button_toast para el atributo android: id, que se usa para identificar el elemento en el layout.

<img src="Medios\17.PNG"/>

Nos va a tirar la siguiente ventana  y le vamos a dar clic en Refactor

<img src="Medios\18.PNG"/>

* Establezca el atributo de background en @color/colorPrimary. (A medida que ingresa @c, aparecen opciones para una fácil selección). Si no está establecido el color, hágalo en colors.xml

<img src="Medios\20.PNG"/> 

<img src="Medios\21.PNG"/>

* Establezca el atributo textColor en @android:color/white.

<img src="Medios\22.PNG"/>

* Edite el atributo text en Toast.

<img src="Medios\23.PNG"/>

* Selecciona el segundo botón y edite su campo id a button_count

<img src="Medios\24.PNG"/>

* Edite el atributo text del segundo botón a Contar

<img src="Medios\25.PNG"/>

* Cambie el color de texto y de fondo a los botones

<img src="Medios\26.PNG"/>

### Agregar el elemento TextView y sus atributos correspondientes

Una habilidad de usar ConstraintLayout es que puedes agregar elementos en cualquier parte del espacio disponible y establecer sus restricciones con cualquier elemento próximo al que se está agregando.

* Desde el panel Palette y el apartado Common, agregue un elemento View TextView y establezca el atributo id a show_count.

<img src="Medios\27.PNG"/>

<img src="Medios\28.PNG"/>

Luego de cambiar el nombre nos va a enviar una ventana de rename y le damos Refactor.

<img src="Medios\29.PNG"/>

* Establezca las restricciones del TextView, la parte superior con el botón de Toast y su parte inferior con el botón contador.

<img src="Medios\27.PNG"/>

* Establezca las restricciones izquierda y derecha del elemento TextView al lado correspondiente al contenedor padre.

<img src="Medios\27.PNG"/>

* Establezca el valor text a 0

<img src="Medios\30.PNG"/>

* Establezca el valor textSize a 160sp

<img src="Medios\31.PNG"/>

<img src="Medios\32.PNG"/>

* Establezca el textStyle a bold

<img src="Medios\33.png"/>

* Cambie layout_width y layout_height a match_constraint

<img src="Medios\34.png"/>

<img src="Medios\35.PNG"/>

* Establezca el textColor a @color/colorPrimary

<img src="Medios\36.PNG"/>

* Establezca un valor preferido al atributo background, opcional el #0F49CD

<img src="Medios\37.PNG"/>

* Establezca el valor gravity a center_vertical

<img src="Medios\38.PNG"/>

### Tarea 1.4: Editando el layout en el XML

¡El diseño de la aplicación Hello Toast está casi terminado! Sin embargo, aparece un signo de exclamación junto a cada elemento de la interfaz de usuario en el árbol de componentes (Component Tree). Pase el puntero sobre estos signos de exclamación para ver los mensajes de advertencia, como se muestra a continuación. Aparece la misma advertencia para los tres elementos: las cadenas codificadas deben usar recursos.

Edite el fichero strings.xml que se encuentra en la carpeta res/values:

Siga los siguientes pasos:

* Abra el fichero activity_main.xml y cambie el modo solamente a código

<img src="Medios\39.PNG"/>

* Cambie el valor de text del TextView a un @string/count_initial_value

