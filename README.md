# Taller-de-nivelacion
Brayan Stiven Zamora Arias

Parte Teórica:
1.	¿Cuáles son los tipos de datos primitivos en Java? 

R// En Java, los tipos de datos primitivos son aquellos que almacenan valores simples y no son objetos. Hay ocho tipos de datos primitivos en Java:

-	byte: 8 bits, almacena valores enteros de -128 a 127.
-	short: 16 bits, almacena valores enteros de -32,768 a 32,767.
-	int: 32 bits, almacena valores enteros de -2,147,483,648 a 2,147,483,647.
-	long: 64 bits, almacena valores enteros de -9 cuatrillones a 9 cuatrillones (requiere una 'L' al final, por ejemplo: 100000L).
-	float: 32 bits, almacena valores decimales de precisión simple (requiere una 'F' al final, por ejemplo: 3.14F).
-	double: 64 bits, almacena valores decimales de precisión doble (se usa por defecto en Java para números con decimales).
-	char: 16 bits, almacena un único carácter Unicode (por ejemplo: 'A', '7', '\u0021').
-	boolean: 1 bit, almacena solo true o false.

2.	¿Cómo funcionan las estructuras de control de flujo como if, else, switch y bucles en Java? 

R// 
Estructuras condicionales:
Se utilizan para ejecutar bloques de código dependiendo de condiciones.

1.	if – else if – else:
Permite evaluar una condición y ejecutar diferentes bloques de código según el resultado.

int num = 11;

if (numero > 0) {
    System.out.println("El número es positivo");
} else if (numero < 0) {
    System.out.println("El número es negativo");
} else {
    System.out.println("El número es cero");
}

2. switch: 
Se usa cuando hay varias opciones posibles para un mismo valor, usando un “break” para evitar que los casos siguientes también se ejecuten.

int dia = 2;

switch (dia) {
    case 1:
        System.out.println("Lunes");
        break;
    case 2:
        System.out.println("Martes");
        break;
    case 3:
        System.out.println("Miércoles");
        break;
    default:
        System.out.println("Día no válido");
}

Bucles (Estructuras de repetición):
Se utilizan para ejecutar un bloque de código varias veces.

1.	for:
Se usa cuando se conoce el número exacto de repeticiones.

for (int i = 1; i <= 5; i++) {
    System.out.println("Iteración: " + i);
}

2.	while:
Se usa cuando la cantidad de repeticiones no es fija, sino que depende de una condición.
int i = 1;
while (i <= 5) {
    System.out.println("Valor de i: " + i);
    i++;
}
3.	do-while:
Es similar a while, pero garantiza que el código se ejecutará al menos una vez, ya que la condición se evalúa después.

int i = 1;
do {
    System.out.println("Valor de i: " + i);
    i++;
} while (i <= 5);


3.	¿Por qué es importante usar nombres significativos para variables y métodos? 

R// Usar nombres significativos para variables y métodos en Java es fundamental porque mejora la legibilidad, mantenibilidad y comprensión del código. Algunas razones clave son:

-	Facilita la comprensión del código.
-	Mejora la mantenibilidad del código.
-	Hace que el código sea más autodescriptivo.
-	Facilita la depuración y evita errores.
-	Buenas prácticas en nombres.

4.	¿Qué es la Programación Orientada a Objetos (POO)? 

R// La Programación Orientada a Objetos (POO) es un paradigma de programación, esto es, un modelo o un estilo de programación que proporciona unas guías acerca de cómo trabajar con él y que está basado en el concepto de clases y objetos. Este tipo de programación se emplea para estructurar un programa de software en piezas simples y reutilizables de planos de código (clases) para crear instancias individuales de objetos.

5.	¿Cuáles son los cuatro pilares de la Programación Orientada a Objetos? 

R// Los cuatro pilares de la Programación Orientada a Objetos (POO) son Encapsulamiento, Herencia, Polimorfismo y Abstracción. Estos conceptos permiten crear código más modular, reutilizable y fácil de mantener en Java y otros lenguajes orientados a objetos. 


6.	¿Qué es la herencia en POO y cómo se utiliza en Java?

R// La herencia en Programación Orientada a Objetos (POO) es un mecanismo que permite que una clase herede atributos y métodos de otra, promoviendo la reutilización del código y facilitando su mantenimiento.

En Java, la herencia se implementa con la palabra clave extends. Se define una superclase (clase padre o base) con atributos y métodos generales. Luego, una subclase (clase hija o derivada) hereda esos atributos y métodos sin necesidad de volver a definirlos.

7.	¿Qué son los modificadores de acceso y cuáles son los más comunes 
en Java? 

R// Los modificadores de acceso en Java son palabras clave que determinan la visibilidad y el nivel de acceso de atributos, métodos y clases dentro de un programa. Permiten controlar el alcance de los elementos de una clase y protegen los datos del acceso indebido.

1. private (Privado)
- Solo accesible dentro de la misma clase.
- No se hereda en subclases.
- Se usa para ocultar datos y protegerlos del acceso externo.

2. (Sin modificador) o "default" (Paquete privado)
- Accesible dentro de la misma clase y el mismo paquete.
- No accesible en subclases fuera del paquete.
- Se usa cuando los elementos solo deben ser visibles dentro del mismo paquete.

3. protected (Protegido)
- Accesible dentro de la misma clase, mismo paquete y en subclases (incluso si están en otro paquete).
- Se usa en herencia para que las subclases puedan acceder a los atributos o métodos de la superclase.

4. public (Público)
 - Accesible desde cualquier parte del programa.
 - Se usa para métodos y atributos que deben ser visibles para todos.



8.	¿Qué es una variable de entorno y por qué son importantes para Java o la programación en general?

R// Una variable de entorno es una configuración del sistema operativo que almacena información importante accesible por programas y procesos.

En Java y en programación en general, las variables de entorno permiten configurar el entorno de ejecución de un programa sin necesidad de modificar el código fuente.

Son importantes por qué:

-	Facilitan la configuración del entorno de desarrollo sin modificar el código.
-	Permiten portabilidad al definir configuraciones independientes del sistema.
-	Mejoran la seguridad al evitar exponer información sensible en el código (Ejemplo: claves API en ENV en Docker).
-	Optimización del desarrollo al automatizar configuraciones para diferentes entornos (desarrollo, prueba, producción).

