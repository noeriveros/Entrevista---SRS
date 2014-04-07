Entrevista---SRS
================































Especificación de requisitos de software

Proyecto: [Proyecto Cookbooks]
Revisión [1.00]


















		[Abril de 2014]
 
Ficha del documento


Fecha	Revisión	Autor	Verificado
[01/04/2014]	[1.00]	[Descripcion]
[Firma o sello]























Documento validado por las partes en fecha: 07/04/2014

Por el cliente	Por la empresa suministradora
	






Aclaración [Nombre]
Aclaración [Nombre]





















 




















 
Contenido
FICHA DEL DOCUMENTO	3
CONTENIDO	4
1	INTRODUCCIÓN	6
1.1	Propósito	6
1.2	Alcance	6
1.3	Definiciones, acrónimos y abreviaturas	6
1.4	Referencias	6
1.5	Resumen	6
2	DESCRIPCIÓN GENERAL	6
2.1	Perspectiva del producto	6
2.2	Funcionalidad del producto	6
2.3	Características de los usuarios	6
2.4	Restricciones	7
2.5	Suposiciones y dependencias	7
2.6	Evolución previsible del sistema	7
3	REQUISITOS ESPECÍFICOS	7
3.1	Requisitos comunes de los interfaces	7
3.1.1	Interfaces de usuario	7
3.1.2	Interfaces de hardware	8
3.1.3	Interfaces de software	8
3.1.4	Interfaces de comunicación	8

3.2	Requisitos funcionales	7

3.3	Requisitos no funcionales	8
3.3.1	Requisitos de rendimiento	8
3.3.2	Seguridad	8
3.3.3	Fiabilidad	9
3.3.4	Disponibilidad	9
3.3.5	Mantenibilidad	9
3.3.6	Portabilidad	9
3.4	Otros requisitos	9
4	APÉNDICES	9

Introducción

Propósito


         El propósito del presente documento es brindar una descripción detallada del sistema, señalando todas y cada una de sus características, incluyendo las funcionalidades, la interface, las condiciones con las que opera, etc. Está dirigido a los dueños de CookBooks que requieren los servicios de Solidez  Informática S.A. para la sistematización de las actividades de ventas de libros.
Alcance


      El sistema se denomina “CookBooks” y tiene como finalidad brindarle al cliente la organización, gestión y administración de la venta de los libros de cocina. Lo cual, una vez funcionando le será útil no solo para obtener información de la venta, sino también para la búsqueda o alguna modificación sobre el libro.

Definiciones, acrónimos y abreviaturas

•	ABM: Alta, baja y modificación de registros de una base de datos.
•	AB: Alta y baja de registros de una base de datos.
•	Casos de Uso: Descripción detallada de todas las funcionalidades del sistema que requieren de la interacción de un usuario con el sistema.
•	CU: Caso de Uso.
•	UF: Unidad Funcional.
•	Distribución: Versión del sistema operativo.


1.1	Referencias
Referencia	Titulo	Fecha	Autor
1	Entrevista	07/04/14	Solidez Informatica  S.A.
2	IEEE 830 Especificación de Requerimientos de Software	07/04/14	IEEE

Resumen


	En el presente documento se describen detalladamente las funcionalidades a desarrollar en la pagina de ventas de libros por internet.
	En principio se realiza una descripción general del mismo, incluyendo un resumen de las funcionalidades más importantes, descripción de los usuarios, las restricciones y evolución de la pagina. También se realizará la descripción detallada de los requerimientos funcionales y no funcionales.


Descripción general
Perspectiva del producto

El sistema que se desarrollará es un producto autónomo e independiente.
Funcionalidad del producto

La pagina permitirá:

•	Ver libros.
•	Buscar libro por autor.
•	Buscar libro por nombre.
•	Crear cuenta.
•	Iniciar sesión.
•	Cerrar sesión.
•	Modificar datos de cuenta.
•	Eliminar cuenta.
•	Visualizar carrito de compra.
•	Agregar libro a carrito.
•	Eliminar libro del carrito.
•	Comprar un libro.
•	Cancelar compra.
•	Agregar un libro de la página.
•	Modificar datos del libro.
•	Eliminar un libro de la página.
•	Modificar estado de una compra.
•	Solicitar informes. 
•	Agregar un autor.
•	Modificar datos del autor.
•	Eliminar autor.
•	Solicitar contraseña en caso de olvido.

1.2	Características de los usuarios
Tipo de usuario	Administrador
Formación	Escaso conocimientos de manejo de PC
Actividades	- Alta, baja y modificación de Autores
- Alta, baja y modificación de Libros
- Ver , Buscar un libro
- Alta y modificación de pedidos
-Solicitar informes
Tipo de usuario	Usuario Visitante
Formacion	Conocimientos de manejo de PC
Actividades	- Ver los libros en el catalogo
- Buscar un libro por nombre o por autor
- Registrarse como cliente en la pagina
Tipo de usuario	Usuario Cliente
Formacion	Conocimientos de manejo de PC
Actividades	- Ver los libros en el catalogo
- Buscar un libro por nombre o por autor
- Comprar libro
- Ver carrito
- Agregar y eliminar libros del carrito
- Modificar sus datos personales
- Desuscribirse de la pagina

Restricciones
         El sistema:
•	Funcionará para sistemas operativos bajo entorno gráfico Windows Xp, Vista o Seven.
•	Correrá correctamente sobre los siguientes navegadores web:
•	Google Chrome 5.0 o superior.
•	Mozilla Firefox 3.5 o superior.
•	Opera 10 o superior.
•	Internet Explorer 8 o superior.
•	Deberá estar disponible las 24hs.
•	Será desarrollado haciendo uso de Delphi 2010 y del motor de bases de datos SQL server.
•	Funcionara correctamente en equipos con los siguientes requisitos mínimos: 
•	Procesador de 32 bits (x86) o 64 bits (x64) a 1 gigahercio (GHz) o más. 
•	Memoria RAM de 1 gigabyte (GB) (32 bits) o memoria RAM de 2 GB (64 bits). 
•	Espacio disponible en disco rígido de 16 GB (32 bits) o 20 GB (64 bits). 
•	Dispositivo gráfico DirectX 9 con controlador WDDM 1.0 o superior. 
Suposiciones y dependencias

La empresa no se responsabiliza por el servidor donde será montado el sistema, ya que no depende de nosotros, sino del servicio que se desee contratar. No obstante, recomendamos el uso de “DattaTei” con el cual  venimos trabajando desde hace siete años y no hemos sufrido inconvenientes con el montaje de nuestros sistemas.
Evolución previsible del sistema

	Venta de libros virtuales.
	Categorias.
	Asociarse a editoriales.
	Manejar proveedores.
Requisitos específicos
Requisitos comunes de los interfaces
Interfaces de usuario

El sistema presentará varias pantallas. Al ingresar se mostrará una pantalla principal en donde se puede visualizar los libros, hacer búsqueda, inicio de sesión, contacto…….
Una vez efectuado el inicio de sesión se visualizara un top menú donde se podrá acceder a las operaciones posibles del sistema correspondiente a la compra de libros, ver catalogos, agregar o cancelar un libro al carrito de compra, modificar datos personales….
Interfaces de hardware

		N/A

Interfaces de software

	N/A
Requisitos funcionales 
 
Serán descriptos como Historias de Usuario.
Requisitos no funcionales
Requisitos de rendimiento

El sistema permitirá cargar un registro de venta  en menos de 10  segundos.
El 95% de las transacciones el motor de base de datos las ejecutará en menos de un segundo.
La visualización del listado de ventas por pantalla no deberá exceder de los veinte segundos.
Seguridad

Los usuarios que acceden al sistema tendrán su nombre de usuario y contraseña. La contraseña caducará cada un año.
La contraseña de administrador pasados los tres intentos fallidos será bloqueado su acceso.
La información en la base de datos se guardará cifrada.
Fiabilidad

         El sistema garantiza menos de 8 errores por cada 1000 transacciones realizadas.
Disponibilidad

               El sistema deberá estar disponible las 24 horas, los 365 días del año.
Mantenibilidad

El sistema será instalado y puesto en marcha por los desarrolladores. Luego de la finalización del período de garantía, el cliente contará con un servicio de mantenimiento cuyas características, precio y forma de pago se detallarán más tarde en otro documento.
Portabilidad
N/A
Otros requisitos

•	El sistema cumplirá con la ley 25.326 Protección de datos Personales.
Apéndices
	N/A
