# Resumen

Variables estáticas

Es una variable que ha sido ubicada estáticamente y cuyo tiempo de vida se extiende durante toda la ejecución del programa.
Las variables estáticas en C tienen las siguientes dos propiedades:
	1.	No pueden ser accedidas desde otro fichero. Por tanto, los prefijos “extern” y “static” no pueden ser utilizados en la misma declaración.
	2.	Mantienen su valor a lo largo de toda la ejecución del programa independientemente del ámbito en el que estén   definidas.
  Como consecuencia de estas dos propiedades se derivan los siguientes casos:
    1.	Si una variable estática está declarada fuera de las funciones, será accesible únicamente por el código que le siga      en el mismo fichero de su declaración.
    2.	Si una variable estática está declarada en una función, sólo será accesible desde esa función y mantendrá su valor       entre ejecuciones de la función.
  Este comportamiento es contra intuitivo porque estas variables se declaran en el mismo lugar que el resto de variables en    una función, pero mientras que estas adquieren valores nuevos con cada ejecución, las estáticas conservan estos valores      entre ejecuciones.

Memoria dinámica

  Es la memoria que se reserva en tiempo de ejecución. Se utiliza cuando no se conoce el número de datos/elementos a usar, El   espacio de memoria asignado a una variable generada de manera dinámica se crea durante la ejecución del programa (tiempo de   ejecución), debido a esto presenta la desventaja de que es más lenta puesto que no se conoce desde un inicio el tiempo de    ejecución. Cuando un programa solicita memoria dinámica para una variable, se le asigna memoria del segmento denominado      montículo o heap.

Clase

  Es una plantilla que define las variables y los métodos que son comunes para todos los objetos de un cierto tipo. Cada       objeto creado a partir de la clase se denomina instancia de la clase. Utilizando un símil con el lenguaje, si las clases     representan sustantivos, los campos de datos pueden ser sustantivos o adjetivos, y los métodos son los verbos.

Objeto

  Un objeto no es más que un conjunto de variables (o datos) y métodos (o funciones) relacionados entre sí. Los objetos en     programación se usan para modelar objetos o entidades del mundo real (el objeto hijo, madre, o farmacéutica, por ejemplo).   Un objeto es, por tanto, la representación en un programa de un concepto, y contiene toda la información necesaria para      abstraerlo: datos que describen sus atributos y operaciones que pueden realizarse sobre los mismos.

Instanciación

  Se refiere a una realización específica de una clase o prototipo determinados. En general, cuando se ejecuta un programa en   un computador, se dice que éste se instancia. En lenguajes que crean objetos a partir de clases, un objeto es una instancia   de una clase. 
  En un mismo proyecto se puede tener una o más instancias de una misma clase. Cada vez que se crea una nueva instancia, ésta   adquiere las propiedades, métodos y eventos de la clase a la que pertenece sin embargo, cada instancia es independiente de   las otras; dos ventajas son:
    1.	Si se hace algún cambio en la clase, todas las instancias de esta clase se actualizarán automáticamente; lo que          permite hacer cambios sin tener que ir a cada una de las instancias.
    2.	Al ser independientes de las otras instancias, se les puede dar valores diferentes sin que afecten a las demás.       Aunque comparten la misma estructura, pueden programarse individualmente, dando versatilidad y flexibilidad al código.

Sobrecarga

  La sobrecarga se refiere a la posibilidad de tener dos o más funciones con el mismo nombre pero funcionalidad diferente,     pero siempre que su lista de argumentos sea distinta. Es decir, dos o más funciones con el mismo nombre realizan acciones    diferentes. El compilador usará una u otra dependiendo de los parámetros usados. A esto se llama también sobrecarga de       funciones. 

Ensombrecimiento

  Una variable local puede llevar el mismo nombre que una variable de instancia, a esto se le conoce como ensombrecimiento     (shadowing).
  “When two programming elements share the same name, one of them can hide, or shadow, the other one. In such a situation,     the shadowed element is not available for reference; instead, when your code uses the element name, the compiler resolves   it to the shadowing element.”

Ciclo de vida de las variables

  El ciclo de vida de una variable nos permite especificar durante cuánto tiempo el contenido de una variable estará            disponible a lo largo de la ejecución de la aplicación.
    •	Variables de instancia
        o	Se crea cuando se crea el objeto que las contiene
        o	Se destruyen cuando el recolector de basura de Java no encuentra referencias activas para el objeto
    •	Variables estáticas
        o	Se crean cuando la clase se usa por primera vez
        o	Suelen existir para el resto del programa
        o	Están accesibles durante toda la duración del funcionamiento de la aplicación
    •	Variables locales
        o	Se crean en la sentencia en la que están definidas
        o	Se destruyen al salir del bloque
    •	Variables de clase
        o	Puede ser utilizada mientras esté disponible en una instancia de la clase

