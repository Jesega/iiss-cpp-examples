# Ejercicios

## Procedimiento

1. Elegir un tema de teoría de la [lista de temas](#temas).
   - Notificar por correo del campus al profesor de teoría el tema elegido y esperar su confirmación.
   - Elegir el ejemplo del tema estudiado en clases de teoría, o bien proponer un ejemplo alternativo.
2. Implementar el ejemplo empleando los mecanismos del lenguaje que se proponga.
   - Incluir una breve explicación escrita en [markdown](https://en.wikipedia.org/wiki/Markdown), que incluya instrucciones sobre cómo compilar el ejemplo.
   - Incluir en el código un programa principal breve de demostración del ejercicio.
   - Ubicar los ficheros markdown y el código fuente del ejemplo en la  carpeta con el nombre del tema situada bajo la carpeta `temas`.
3. Publicar el ejemplo en este mismo repositorio
   - Añadir todos los cambios en una rama (_branch_) con el mismo nombre del tema, en minúsculas y sin acentos. 
   - Todos los ficheros deben estar realizados sobre una carpeta cuyo nombre también coincida con el nombre del [tema](#temas).
   - Los nombres permitidos para las carpetas a situar bajo `temas/` son: `ocultacion`, `herencia`, `delegacion`, `functors`, `anotaciones`, `undefined`, `aspectos`, `lambdas`, `mixins`.
   - Los cambios deben incluir las instrucciones, el código realizado y los ficheros de configuración y makefiles necesarios para compilar y probar el ejemplo.
   - Al acabar el ejercicio, hacer una [solicitud de extracción](https://docs.github.com/es/github/collaborating-with-issues-and-pull-requests/about-pull-requests) o [pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests) (PR) en la rama creada con el nombre del tema para solicitar la incorporación de lo realizado en el ejercicio. 
   - Instrucciones: [¿Cómo hacer tu primer pull request en Github?](https://www.freecodecamp.org/espanol/news/como-hacer-tu-primer-pull-request-en-github/)
   - No olvides borrar la rama que has empleado para hacer el PR del tema elegido.
4. Hacer la presentación del ejercicio realizado de alguna de estas dos formas:
    - Pedir fecha al profesor para presentar el ejemplo en clase, o bien...
    - Grabar un video explicativo de menos de 8' y entregarlo a través del [campus](https://av03-20-21.uca.es/moodle/mod/assign/view.php?id=91252).

## Temas

### 1. Ocultación

Implementar en C++ el ejemplo final de [Recorrido de listas](http://dodero.github.io/iiss/iiss-oop-1/#implementacion-alternativa-lista-v04) usando los siguiente mecanismos de ocultación de la implementación en C++:

- Modificadores de visibilidad: `protected`, `private`, `friend`
- Iteradores de `std`

> Referencias: Capítulo 5 de _Bruce Eckel-Thinking in C++_

### 2. Herencia

Implementar en C++ el ejemplo de [Aventura](http://dodero.github.io/iiss/iiss-oop-1/#ejemplo-aventura-v01) usando los siguientes mecanismos de C++:

- Herencia simple
- Dynamic casting

>  Referencias: Capítulo 14 de _Bruce Eckel-Thinking in C++_


### 3. Delegación 

Implementar en C++ el ejemplo final de [Orquesta](http://dodero.github.io/iiss/iiss-oop-2/#implementacion-alternativa-orquesta-v06) usando los siguientes mecanismos de C++ para la delegación/composición: 

- Métodos polimórficos
- Funciones virtuales

> Referencias: Capítulo 15 de _Bruce Eckel-Thinking in C++_

### 4. Functors

 Implementar en C++ el ejemplo de la identificación de [BankAccount](http://dodero.github.io/iiss/iiss-oop-3/#ejercicio-identificador-de-bankaccount-con-inyeccion-de-dependencias) y que se puedan definir diversos atributos para comparar cuentas, usando los siguientes mecanismos de C++ para inyectar como dependencias el criterio de comparación:

- polimorfismo paramétrico (_templates_)
- sobrecarga de operadores binarios
- objetos función o _functors_
 
> Referencias:
>  - Capítulo 16 de _Bruce Eckel-Thinking in C++_
>  - Capítulo 12 de _Bruce Eckel-Thinking in C++_
>  - [Functors](https://www.cprogramming.com/tutorial/functors-function-objects-in-c++.html) en C++

### 5. Anotaciones

Implementar en Java el ejemplo de [BankAccount](http://dodero.github.io/iiss/iiss-oop-3/#ejercicio-identificador-de-bankaccount-con-inyeccion-de-dependencias) con diversos atributos comparables, usando los siguientes mecanismos de Java para inyectar como dependencia el comparador a usar:

- anotaciones definidas a medida según el [JSR 330](http://javax-inject.github.io/javax-inject/) 

> Referencia: [Creating a Custom Annotation in Java](http://baeldung.com/java-custom-annotation) de Baeldung

### 6. Excepciones

Implementar en Java ejemplos de excepciones, usando los siguientes mecanismos para gestión de errores:

- Excepciones checked en Java
- Excepciones unckeched en Java

> Referencias:
>  - Capítulo XX de _Bruce Eckel-Thinking in C++_


### 7. Undefined

Implementar en C++ el ejemplo del caso "MobileTester" del apartado [Optionals](http://dodero.github.io/iiss/iiss-err/#optionals) usando los siguientes mecanismos del lenguaje para resolver el problema de los valores no definidos y el mal uso de `null`:

- `std::optional`

> Referencia: [CppReference](https://en.cppreference.com/w/cpp/utility/optional)

### 8. Aspectos

Implementar en C++ usando aspectos el ejemplo del caso [Editor de Figuras](http://dodero.github.io/iiss/iiss-aop/#caso-5-editor-de-figuras).

> Referencia: [AspectC++](https://www.aspectc.org/)


### 9. Lambdas

Implementar ejemplos en C++ del uso de funciones anónimas (expresiones _lambda_) empleando los siguientes mecanismos del lenguaje:

- Lambdas genéricas de C++11
- Lambdas variádicas de C++14/C++17
- Lambdas mutables 

> Referencias:
>  - [All About Lambda Functions in C++](https://dzone.com/articles/all-about-lambda-functions-in-cfrom-c11-to-c17)
>  - [Lambdas: From C++11 to C++20: Part 1](https://www.bfilipek.com/2019/02/lambdas-story-part1.html)
>  - [Lambdas: From C++11 to C++20: Part 2](https://www.bfilipek.com/2019/03/lambdas-story-part2.html) + 

### 10. Mixins

Implementar en C++ un ejemplo de _mixin_ que permita mezclar distintos comportamientos en una misma clase, empleando los siguientes mecanismos del lenguaje:

- polimorfismo estático (templates)
- polimorfirmo dinámico

> Referencias:
>  - [DrDobbs Journal](https://www.drdobbs.com/cpp/mixin-based-programming-in-c/184404445)
>  - [Combining Static and Dynamic Polymorphism with C++ Mixin classes](https://michael-afanasiev.github.io/2016/08/03/Combining-Static-and-Dynamic-Polymorphism-with-C++-Template-Mixins.html)


### 11. Promesas

Implementar en C++ un ejemplo de programación asíncrona, similar a los mostrados en [Promesas y futuros](http://dodero.github.io/iiss/iiss-evp-2/#promesas), que emplee los siguientes mecanismos del lenguaje:

- `std::async`
- `std::promise`

> Referencias:
>   - [CppReference: thread support library](https://en.cppreference.com/w/cpp/thread)
>   - [CppReference: async](https://en.cppreference.com/w/cpp/thread/async)
>   - [CppReference: promise](https://en.cppreference.com/w/cpp/thread/promise)

### 12. Futuros

Implementar en C++ un ejemplo de programación asíncrona, similar a los mostrados en [Promesas y futuros](http://dodero.github.io/iiss/iiss-evp-2/#promesas), que emplee los siguientes mecanismos del lenguaje:

- `std::async`
- `std::future`

> Referencias:
>   - [CppReference: thread support library](https://en.cppreference.com/w/cpp/thread)
>   - [CppReference: async](https://en.cppreference.com/w/cpp/thread/async)
>   - [CppReference: future](https://en.cppreference.com/w/cpp/thread/future)

### 13. Variants

Implementar en C++17 un ejemplo de uso de uniones type-safe empleando los siguientes mecanismos del lenguaje:

- `std::variant`

> Referencias:
>  - [CppReference: variant](https://en.cppreference.com/w/cpp/utility/variant)
>  - [Everything You Need to Know About std::variant from C++17](https://www.bfilipek.com/2018/06/variant.html)

### 14. Observables

Implementar en C++ un ejemplo de procesamiento de streams de eventos asíncronos empleando los siguientes elementos de la biblioteca [RxCpp](https://github.com/ReactiveX/RxCpp):

- `rxcpp::observable`

>  Referencias:
>  - [ReactiveX.io](http://reactivex.io/intro.html)
>  - [Observables de RxCpp](http://reactivex.io/RxCpp/index.html)
