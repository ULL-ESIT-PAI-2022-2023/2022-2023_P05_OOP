# Práctica 5. Programación Orientada a Objetos en TypeScript
### Factor de ponderación: 6

### Objetivos
Los objetivos de esta práctica son:
* Poner en práctica metodologías y conceptos de Programación Orientada a Objetos en Script.
* Poner en práctica Principios y Buenas prácticas de programación Orientada a Objetos.

### Rúbrica de evaluacion del ejercicio
Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva)
que se tendrán en cuenta a la hora de evaluar esta práctica:
* Se valorará la realización de las diferentes tareas que se proponen
* El comportamiento del programa debe ajustarse a lo solicitado en este enunciado.
* Capacidad de la programadora de introducir cambios en el programa desarrollado.
* Conocer y poner en prácticas los principios y buenas prácticas de programación orientada a objetos.
* Saber corregir bugs en sus programas utilizando el depurador de Visual Studio Code
* Deben usarse estructuras de datos adecuadas para representar los diferentes elementos que intervienen en el problema
* Ser capaz de desarrollar programas simples en TypeScript en el entorno Linux de la VM de la asignatura usando
  `ts-node`
* Ser capaz de generar documentación para sus programas TypeScript utilizando
  [TypeDoc](https://typedoc.org/)
  y de visualizar dicha documentación en un servidor web
* El alumnado debe ser capaz de resolver problemas tanto en JS como en TS en la plataforma Exercism subiendo sus soluciones a la misma.
* Ser capaz de desarrollar tests unitarios para sus programas utilizando
  [Jest](https://jestjs.io/)
* Acreditar su capacidad para configurar y utilizar 
  [ESLint](https://eslint.org/)
y que es capaz de trabajar con la misma en Visual Studio Code.
* Acreditar que conoce las etiquetas de 
  [JSDoc](https://jsdoc.app/)
* Acreditar que es capaz de generar documentación para sus programas utilizando
  [TypeDoc](https://typedoc.org/)
y que es capaz de generar documentación para sus programas utilizando la herramienta.
* El alumnado ha de acreditar que es capaz de desarrollar programas de la plataforma Jutge
* Se comprobará que el código que el alumnado escribe se adhiere a las reglas de las Guías de Estilo de Google
  para Javascript y/o TypeScript
* Todas las prácticas realizadas hasta la fecha, incluída la que se presenta para su evaluación, se encuentran alojadas en repositorios privados de GitHub.
* Acreditar que es capaz de editar ficheros de forma remota en su VM usando Visual Studio Code

### Indicaciones de caracter general
En esta práctica y las siguientes se promoverá el uso del paradigma orientado a objetos.
Los programas han de organizarse en torno a clases que se han de implementar usando la sintaxis para
clases ES6 de JavaScript y poniendo en práctica los principios de abstracción y encapsulamiento característicos 
de la Programación Orientada a Objetos.
En los ejercicios han de ponerse en práctica los principios y buenas prácticas que han sido expuestos en las clases de la asignatura.

Vigile siempre el tipo de visibilidad que elige para los atributos (properties) de sus clases
y tenga en cuenta tanto las reglas de 
[estilo](https://google.github.io/styleguide/jsguide.html#features-classes)
como las 
[etiquetas JSDoc](https://stackoverflow.com/questions/41715994/how-to-document-ecma6-classes-with-jsdoc)
relacionadas con el constructo `class`.

Previo a la implementación de cada clase, diseñe y desarrolle un conjunto de tests para probar el correcto
funcionamiento de todos los métodos públicos.

Encapsule las clases en módulos que exporten la correspondiete clase hacia otros programas clientes que pudieran utilizarla.

Configure para la práctica una página web que sirva de índice para mostrar la documentación generada por
JSDoc para todos los ejercicios de la práctica.

Configure un fichero `package.json` en el directorio raíz de su repositorio de modo que ejecutando 
`npm install` queden instaladas todas las dependencias de su proyecto.












## Introducción a TypeScript

### Ejercicios simples de TypeScript en Exercism
Únase al
[TypeScript track in Exercism](https://exercism.org/tracks/typescript)
y realice en él todos los ejercicios que sea capaz, particularmente aquellos que ya haya realizado en JavaScript.
Del mismo modo que hizo en JS, comience con los problemas más sencillos como **Hello World** o **Two Fer** y progrese
en este itinerario tanto como le sea posible.
De la 
[Ejercicios de TypeScript en Exercism](https://exercism.org/tracks/typescript/exercises)
una vez que haya realizdo algunos de los ejercicios catalogados como fáciles (*Easy*) preste atención a
algunos de los de dificultad media o alta.
Tenga en cuenta que por ahora no se le requerirá trabajar con ejercicios que conlleven programación orientada a objetos.

Todos los ejercicios que realice en TypeScript han de seguir los criterios de formato, estilo y documentación que
se han venido estudiando hasta ahora.
Para el caso de TS recuerde que existe una guía de estilo específica,
[Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)
que para algunos aspectos específicos complementa a la guía de estilo para JS.

En cuanto a documentación de código se seguirán utilizando los mismos criterios y etiquetas de JSDoc que ya
se han estudiado.

Recuerde que Exercism también utiliza Jest como plataforma de testing para los ejercicios de TypeScript.
Para cada problema, preste atención a los tests que su código ha de superar y la implementación de los mismos.

### Unit Testing con Jest
Realice en TypeScript cada uno de los siguientes problemas de
[Jutge](https://jutge.org/)
haciendo que la entrada que requieran los programas que solucionan el problema se tome por línea de comandos.
Para capturar los parámetros de línea de comando ejecutando el programa en `ts-node` pueden seguir usando
`process.argv`

Haga también que los programas incluyan documentación en formato JSDoc (TypeDoc). 
Se propone desarrollar una página *índice* desde la que se enlacen las páginas de documentación de cada uno de
estos programas.

Desarrolle tests unitarios en 
[Jest](https://jestjs.io/)
para probar la corrección de cada una de las soluciones.
Aparte de los tests públicos de Jutge, incluya al menos un test test adicional para comprobar situaciones que
considere relevantes.
Si su solución se basa en varias funciones, desarrolle tests para cada una de ellas.

1. [P34279](https://jutge.org/problems/P34279) Add one Second.
2. [P51126](https://jutge.org/problems/P51126) Intervals (I)
3. [P33839](https://jutge.org/problems/P33839) Sum of Digits. Para este problema, simplifique la salida de
modo que ésta se limite a un único número (la suma de los dígitos).
4. [P80660](https://jutge.org/problems/P80660) The sequence of Collatz
5. [P91173](https://jutge.org/problems/P91173_en) Collatz pseudo-sequences (1)
6. [P11916](https://jutge.org/problems/P11916_en) Approximation of e. Simplifique la salida del programa para
que se limite a un solo número en punto flotante (el valor de e).
7. [P76024](https://jutge.org/problems/P76024_en) Sum of fractions

## TypeDoc
[TypeDoc](https://typedoc.org/)
es una generador de documentación para proyectos TypeScript, similar a JsDoc o javadoc.
Funciona del mismo modo que JSDoc: la herramienta extrae los comentarios de documentación directamente del código fuente
genera un sitio web de documentación HTML para el proyecto.

Para comenzar a usar TypeDoc simplemente ejecute los siguientes comandos:
```
# Install
npm install --save-dev typedoc

# Execute typedoc on your project
npx typedoc src/index.ts
```
Para un conocimiento más exhaustivo de la herramienta revise el vídeo
[Configuración y y uso de TypeDoc](https://drive.google.com/file/d/19LLLCuWg7u0TjjKz9q8ZhOXgbrKtPUme/view)
del profesor 
[Eduardo Segredo](https://portalciencia.ull.es/investigadores/80784/detalle)
y/o el
[TypeDoc Tutorial](https://cancerberosgx.github.io/javascript-documentation-examples/examples/typedoc-tutorial-basic/docs/docco/src/index.html#:~:text=TypeDoc%20is%20an%20API%20documentation,HTML%20documentation%20website%20for%20you.)

Para los problemas 

4. [P80660](https://jutge.org/problems/P80660) The sequence of Collatz
5. [P91173](https://jutge.org/problems/P91173_en) Collatz pseudo-sequences (1)
7. [P76024](https://jutge.org/problems/P76024_en) Sum of fractions

del apartado anterior, genere con TypeDoc la documentación en formato HTML para cada uno de estos programas y haga que dicha documentación 
sea accesible a través de un servidor web en su máquina virtual de la asignatura.

## Referencias
* [Exercism](https://exercism.io/)
* [Introduction to TypeScript](https://github.com/alu0101329888/Introduction-to-TypeScript)
* [TypeScript Tutorial](https://www.typescripttutorial.net/)
* [TSConfig Reference](https://www.typescriptlang.org/tsconfig)
* [TypeDoc](https://typedoc.org/)
* [TypeDoc Tutorial](https://cancerberosgx.github.io/javascript-documentation-examples/examples/typedoc-tutorial-basic/docs/docco/src/index.html#:~:text=TypeDoc%20is%20an%20API%20documentation,HTML%20documentation%20website%20for%20you.)
* [TypeScript track in Exercism](https://exercism.org/tracks/typescript)
* [Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)
* [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)
* [Jutge web site](https://jutge.org/)
* [Jest](https://jestjs.io/)
* [ESLint](https://eslint.org/)
* [JSDoc](https://jsdoc.app/)
