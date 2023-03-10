<p align="center">
<h1 align="center">Repositorio: Primer Proyecto En GitHub Arekusandora y Nat Vergara</h1>
<div align="center"><img src="https://i.pinimg.com/564x/7d/a2/ab/7da2abca1de4d6219dee0d9407f67e9b.jpg"></div>
</p>
<p align="center">
<h3 align="center">¡Holi, Bienvenido A Nuestro Repositorio!</h3>
</p>
<p align="center"> ¡Nos alegra mucho que estés aquí! Por eso intentamos diseñar un ReadMe que fuera muy bonito, para poder contarte un poco de todo esto </p>

<p align="center">--------------------       🖤       --------------------       🖤       --------------------       🖤       --------------------       🖤       --------------------</p>

<p align="center"> No sé si seas consciente de lo importante que es para nosotras este repositorio, a ver, es nuestro primer repositorio diseñado, y administrado solo por nosotras, lo que quiere decir que es algo que aprendimos hace poco jijiji...</p>

<h3 align="center">Y por eso es tan especial 😎</h3>

<p align="center">Bueno, tambien lo hace especial el hecho de que sea el ReadMe del proyecto que probablemente vas a ver a continuacíon :v</p>
<p align="center">Pero esas son cosas menores, pasemos al proyecto...</p>


# Recursos Humanos

Una "Empresa" de recursos humanos nos ha contratado, a nosotras [Nat💙](https://github.com/NatVerB) y [Arekusandora🧛](https://github.com/ArekuInBlueee), para elaborar un programa que le ayude a almacenar y gestionar la información de los candidatos nuevos que la empresa va a recibir. Uno de los requerimientos básicos del programa es que se debe agregar a cada candidato diligenciando obligatoriamente cada uno de los siguientes datos:

 - Nombres

 - Apellidos

 - Cédula

 - Edad

 - Cargo

Sumado a esto, el programa debe poder eliminar, listar y modificar a cada candidato, además de poder listar a todos los candidatos que la empresa tiene registrados. Se requiere que el Software sea elaborado con el patrón MVC, incluya las Clases DAO Y DTO y sea capaz de serializar y deserializar la información.

# Código Fuente del Software

## [Controller:](https://github.com/NatVerB/RecursosHumanosProyecto/tree/main/RecursosHumanosNV/src/co/edu/unbosque/controller)

* [AplMain](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/controller/AplMain.java)

 Esta es la clase Main, la cual llamamos comunmente AplMain, es la clase que contendrá el método que dará "Inicio" como su nombre lo indica, a todo el
 funcionamiento del programa.
 
* [Controller](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/controller/Controller.java)
 
 Esta es la clase Controller, será quien contendrá el metodo controlador que cada una de las clases que el programa pueda necesitar para su correcto funcionamiento.
 
 ## [Model:](https://github.com/NatVerB/RecursosHumanosProyecto/tree/main/RecursosHumanosNV/src/co/edu/unbosque/model)
 
* [CandidatosDAO](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/model/CandidatosDAO.java)
 
Esta es la clase CandidatosDAO, es la que contiene todos los metodos que se van a ejecutar para que el software pueda Agregar, Eliminar, Modificar y Listar a los candidatos correctamente. Un ejemplo de estos métodos es el de listarCandidatos() y listarEspe() En en el que ambos hacen teoricamente lo mismo, pero uno listará a todos los candidatos y el otro listará a el candidato especifico que se consulte por su cédula.

* [CandidatosDTO](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/model/CandidatosDTO.java)

Esta es la clase CandidatosDTO, es en donde crearemos al objeto "Candidatos" con sus respectivas características y atributos, con el fin de poder guardar sus datos y representarlo cuando lo necesitemos ✔.

### [Persistance:](https://github.com/NatVerB/RecursosHumanosProyecto/tree/main/RecursosHumanosNV/src/co/edu/unbosque/model/persistance)

Persistance, es un paquete que creamos dentro del paquete modelo o "Model", ya que tambien trabaja temas de lógica en el software, pero se separa por que se encarga de algo en específico. En nuestro caso será el paquete que contenga las clases de serializado.

* [FileHandler](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/model/persistance/FileHandler.java)

Esta es la clase FileHandler, la cual tiene como función el correcto serializado de la información de los candidatos registrados en el programa 👩‍💻.

Cuenta con dos métodos muy importantes: readSerializable() y writeSerializable(). Estos métodos nos servirán, uno: Para obtener la informacion del candidato, ya añadida al archivo serializado, para luego poder agregarlos nuevos al ejecutar el programa y tener la información válida. Dos: Para escribir la información de los candidatos o las modificaciones realizadas a los mismos en el documento serializado para que se encuentre actualizado.

* [Archivo Serializado](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/model/persistance/Serializable.n)

Lo siguiente que encontrarás en este paquete, será el archivo serializado, este puede crearse directamente desde el Software y será el archivo en el que se guarde o se lea toda la información serializada 🤑.

## [View:](https://github.com/NatVerB/RecursosHumanosProyecto/tree/main/RecursosHumanosNV/src/co/edu/unbosque/view)

Este es el paquete de vista o en nuestro caso "View". Es en el que contendremos todas las clases en las que crearemos todo el código correspondiente de la Interfaz Gráfica del Usuario.

Cada una de las ventanas funcionales de la interfaz gráfica suele tener detras una lógica muy similar 👀, cambia dependiendo de su objetivo y diseño visual, sin embargo la creación de sus objetos y clases Keyy y Action Listener tienen la misma creación y función.

<h3 align="center">Te dejamos a continuación las clases de la GUI por si te interesan:</h3>

- [AgregarCandidato✔](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/view/AgregarCandidato.java)
- [EliminarCandidato❌](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/view/EliminarCandidato.java)
- [ModificarCandidato🔄](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/view/ModificarCandidato.java)
- [ListarCandidatos📄](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/view/ListarCandidatos.java)
- [ListaEspecifica📑](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/view/ListaEspecifica.java)
- [Menu📋](https://github.com/NatVerB/RecursosHumanosProyecto/blob/main/RecursosHumanosNV/src/co/edu/unbosque/view/Menu.java)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Bien, ahora que te hemos explicado un poco mas de que va esto, esperamos que te sea de mucha utilidad esta información y que si así lo necesitas, pueda ayudarte cualquier elemento de este repositorio...

Si todavia tienes dudas, puedes consultar nuestro documento [JavaDoc]() del Software, en donde podrás encontrar absolutamente toda la información acerca del programa.

## Hasta Luego 💋

*ReadMe diseñado y redactado por Alejandra Valero y Natalia Vergara*

*Imagenes tomadas de Pinterest*
