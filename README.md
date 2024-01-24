# Proyecto del curso de Backend de Coderhouse de Daniel Brusatin.

## Avance de proyecto:
* - [x] Desafío 1: Creación de clase ProductManager.
* - [x] Desafío 2: Agregado de fileSystem para tener persistencia en archivo de productos.
* - [x] Desafío 3: Desarrollo de servidor basado en Express para consultar el archivo de productos.
* - [ ] Primera preentrega: Desarrollo de servidor con los endpoints y servicios necesarios para gestionar los productos y carritos de compra en el e-comerce.
  * Router de productos en **/api/products**:
    * Metodo GET en '/' : Muestra los productos con la query de limit.
    * Metodo GET en '/:pid/' : Muestra un producto por su ID, validando que el ID sea un número y que exista un producto con ese ID.
    * Metodo POST en '/' : Agrega un producto con las propiedades pasadas en el body, se comprueba que los campos obligatorios estén presentes y solo se toman las propiedades que necesitamos para el producto.
    * Metodo PUT en '/:pid' : Actualiza las propiedades válidas de un producto, verificando que exista un producto con ese ID; sin modificar el ID.
    * Metodo DELETE en '/:pid' : Elimina un producto verificando que exista uno con ese ID.
  * Router de carritos en **/api/carts**:
    * Metodo POST en '/' : Crea un nuevo carrito con ID único y con un array vacío de productos.
    * Metodo GET en '/:cid' : Muestra los productos de un carrito verificando que exista un carrito con ese ID. Si bien el carrito solo guarda el ID de los productos, se muestran todas las propiedades del producto mas la cantidad del mismo.
    * Metodo POST en '/:cid/product/:pid' : Agrega un producto a un carrito verificando que existan ambos ID, si el producto ya esta en el carrito se le suma 1 a la cantidad.
* - [ ] Desafío 4: Integración al servidor de vistas usando handlebars y sockets con websockets.

