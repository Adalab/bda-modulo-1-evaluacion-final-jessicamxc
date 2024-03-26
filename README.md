Instrucciones de uso del proyecto TiendaOnline:

En este repositorio encontrarás una plantilla de uso para tu Tienda Online, con ella podrás llevar un amplio registro de tu inventario, tus clientes y tus ventas totales.

A continuación les explicaré la utilidad de cada metodo al ejecutarlo:

En primer lugar tiene que instanciar la clase, es decir, dar nombre a su tienda e = (igualar)TiendaOnline(), asi podrá llamar a los metodos.
- Ejemplo: tienda_ropa=TiendaOnline()

Metodo agregar_productos(): Agrega el nombre del producto, junto con el precio y la cantidad que hay en stock. Si intentas agregar un producto ya existente (por el nombre), éste metodo entiende que está actualizando la cantidad de stock.
- Ej: p1 = tienda_ropa.agregar_productos("camisa", 30, 10)

Metodo ver_inventario(): Este método nos muestra el inventario del que disponemos, de una manera mas limpia y ordenada, de fácil lectura, pero mismos detalles que indicamos en el metodo anterior. (nombre, precio y cantidad)
- Ej: Nombre: camisa Precio: $ 30 Cantidad:  10
- Nombre: abrigo Precio: $ 10 Cantidad:  5
- Nombre: pantalon Precio: $ 35 Cantidad:  5
- Nombre: calcetines Precio: $ 4 Cantidad:  2
- Nombre: vestido Precio: $ 40 Cantidad:  10

Metodo buscar_producto("nombre del producto"): Este metodo nos devuelve el nombre y detalles (precio y cantidad de stock) que hemos instanciado a buscar. Solo se puede buscar productos de uno en uno.

Metodo actualizar_stock("nombre del producto", Q): Con este metodo podemos actualizar el stock de un producto en concreto. 

Metodo eliminar_producto("nombre del producto"): Escribimos el nombre del productos a eliminar del stock. Si el producto está en stock, nos devuelve un mensaje: Producto borrado. En el caso que el producto que deseamos eliminar no estuviera en el stock, nos devolverá un mensaje de que el producto no ha sido encontrado para realizar la accion (eliminar).

Metodo calcular_valor_inventario(): Nos devuelve el valor total de nuestro inventario.

Metodo buscar_producto_regex("patron"): Podemos buscar por un patron, en los nombres de nuestros productos, los productos que coincidan serán devueltos en una lista.

Metodo realizar_compra(): Al llamar este metodo, se nos preguntará si queremos realizar una compra , si la respuesta es ;si, se nos muestra el catalogo disponible de la tienda y tendremos que introducir el producto que queremos comprar, así sucesivamente hasta que respondamos que no queremos comprar más. Tras esta respuesta; no, nos muestra un resumen de la compra, con los articulos seleccionados y el precio total de compra.
A su vez este metodo, restará del stock los productos que se han seleccionado.

Metodo procesar_pago(): Al instanciar este metodo nos solicita ingresar el monto de la cuenta a pagar y el importe dado por el cliente. Nos devolverá un mensaje de si la compra se ha realizado con éxito: si hay cambio que devolver al cliente, o si el monto dado por el cliente es insuficiente.

Metodo agregar_cliente("nombre del cliente", "email contacto"):  A traves de este metodo, se creará un diccionario de nuestros clientes con la información de su nombre y email de contacto.

Metodo ver_clientes(): Nos mostrara nuestros clientes registrados, de una manera mas limpia y ordenada, de fácil lectura, pero mismos detalles que indicamos en el metodo anterior. (nombre y email.)

Metodo registrar_compra(): Con este metodo podemos añadir a nuestros clientes ya registrados un historial de compras, en el caso de que sea un cliente nuevo, primero tendremos que agregar_cliente y despues registrar_compra.

Metodo ver_compras_cliente("nombre del cliente"):  Nos mostrará el historial de compras de un cliente en concreto.

Metodo calcular_ventas_totales(): Finalmente con este metodo llevaremos la cuenta del total de ventas de nuestra TiendaOnline.