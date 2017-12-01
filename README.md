# Curso Le�n EOI 2017 C# y DotNetCore
Introducci�n al lenguaje C# y .NET Core por Diego Ponce de Le�n para la EOI

## Herramientas utilizadas

- Dotnet CLI
- Visual Studio Code
- Visual Studio Community edition
- Nuget
- Git por l�nea de comandos
- Git desde Visual Studio Code
- Git desde Visual Studio
- Github
- GitKraken
- Postman

## Conceptos aprendidos durante el desarrollo

### .NET Core

- Introducci�n a .NET Framework
- Introducci�n a .NET Core
- Diferencias entre .NET Framework y .NET Core
- Instalaci�n entorno de trabajo para .NET Core (SDK)
- Crear proyectos de consola, librer�a NET Standard y Web API con .NET Core desde l�nea de comandos (CLI) y desde Visual Studio
- Instalaci�n, configuraci�n y uso de Visual Studio Code para editar proyectos C#
- Instalaci�n, configuraci�n y uso de Visual Studio Community para editar proyectos C#
- Crear dependencias entre proyectos dentro de una misma soluci�n
- A�adir paquetes nuget a un proyecto
- Utilizaci�n de librer�as de terceros a trav�s de nuget
- Depurar c�digo C# en Visual Studio Code
- Depurar c�digo C# en Visual Studio Community
- Interacci�n de usuario (entrada y salida de datos) en un proyecto de Consola

### Git

- Comandos b�sicos de Git desde la l�nea de comandos (add, status, commit, remote add, pull, push)
- Operaciones b�sicas de Git desde Visual Studio Community
- Creaci�n de repositorio Git en GitHub
- Vincular un repositorio Git local con uno remoto en GitHub

### C#

- Value types
- Declaraci�n y utilizaci�n de variables
- Comandos de selecci�n (if, else if, switch)
- Operadores comunes
- Operador ternario
- Comandos de iteraci�n (while, do while, for, foreach)
- Comandos de salto (break, continue)
- Declaraci�n y utilizaci�n de propiedades de clase
- M�todos de clase
- Par�metros de m�todo
- Arrays
- Colecciones
- LINQ + Lambda
- Clases y objetos
- Herencia
- Polimorfismo
- Encapsulaci�n
- M�todos est�ticos
- Async, await, Task
- Lanzamiento y manejo de excepciones

### REST y Web API

- Introducci�n a REST
- M�todos b�sicos REST (get, post, put, delete)
- Probar una API REST con Postman
- Consumir una API REST desde C# con `HttpClient`
- Crear una API REST con Asp.NET Core y Visual Studio
- Usar respuestas de Web API: BadRequest, NoContent, Ok, ServerError, CreatedAtRoute, etc
- Crear un modelo de datos relacional
- Usar inyecci�n de dependencias para el uso de servicios en controladores Web API
- Introducci�n a ORM (Object Relatioinal Mapper)
- Introducci�n al ORM Entity Framework
- Usar base de datos en memoria
- Consultas a la base de datos de forma s�ncrona con LINQ
- Consultas a la base de datos de forma as�ncrona con LINQ


# Ejercicios

## Fight Game

Mini juego de peleas por turnos desarrollado durante las clases. Se trata de una aplicaci�n de consola que descarga lista de personajes desde la API REST de StarWars. 
Cada vez que se teclea la funci�n "Luchar", se eligen dos contrincantes aleatoriamente. El da�o que ocasionan o reciben tambi�n es aleatorio. Todos van perdiedo poder y vidas. 
Cuando se agotan sus vidas quedan fuera de juego. As� sucesivamente hasta que queda un �nico superviviente o ganador.
Tiene otra funci�n "Estatus" con la cu�l podemos ver una tabla de texto de los jugadores y el detalle de cada uno.

La l�gica del juego es muy simplista y esta aplicaci�n ha servido b�sicamente para tocar varios puntos importantes del lenguaje C#, al mismo tiempo que hemos aprendido a manejar entrada y salida de datos en aplicaciones de consola.

![Game screenshot 1](https://raw.githubusercontent.com/xleon/FightGame/master/Screenshot_1.png)
![Game screenshot](https://raw.githubusercontent.com/xleon/FightGame/master/image.png)

## TO DO web API (Lista de tareas)

Se trata de una API REST muy simple, desarrollada en Visual Studio, con dos modelos de datos (lista de tareas y tarea) que est�n relacionados entre s�. 
Hemos hecho un recorrido por los m�todos REST m�s relevantes para entender el concepto CRUD (Create Retrieve Update Delete). Para ello hemos utilizado un servicio que se utiliza en el controlador mediante inyecci�n de dependencias.
En dichos m�todos se controlan errores y que los par�metros recibidos en la llamada sean correctos. Tambi�n se consulta una base de datos con LINQ 
y finalmente se devuelven las respuestas correspondientes y t�picas de REST, con su c�digo de estado y su cuerpo en formato json. Toda la API web ha sido probada con Postman.

