# Prueba Intcomex
Andres Ortiz

Repositorio Publico creado para compartir la prueba.

La documentacion de uso completa se envia via mail.

#Detalles:


#Servicios
#Crear Categoría (  POST    api/crear/categoria/) 
  El servicio de Crear Categoria adiciona una nueva categoria a la tabla categories para ser usada en la creacion posterior de productos. 
  Recibe como queryParams el nombre y la Url de la imagen de la categoria. 

#Crear Producto (  POST    api/crear/producto/)
  El servicio de crear producto llama de manera asyncrona a un storage procedure de la base de datos que es el encargado de generar la información de los 100.000 productos.

#listar productos ( GET	api/listar/productos/)
  El servicio de listar productos recibe como queryParams los key page y limit que corresponden a la pagina que se desea visualizar y la cantidad de productos a presentar por pagina respectivamente.
  Por temas de rendimiento y maquina se realizan pruebas con 3100 productos sin embargo para la revision de esta prueba la version que esta desplegada en cloud tiene configurado llamar al storage procedure indicando los 100.000 productos.

#listar productos por ID (GET    api/listar/ProductoId/)
  Este servicio recibe como queryParam el prodId correspondiente al id del producto a consultar.
  En su response trae la data principal del producto, nombre, id, categoria y la url de la imagen de la categoria. 

#Ping (GET    api/ping)
  Este servicio se crea para validar el status de la api, se crea como un ping alive, en su response brinda:

 
#Despliegue.

La api fue desplegada en ambiente sandbox de mulesoft anypoint platform.

#Url de endpoint: https://intcomex-prueba-oqac94.5sc6y6-3.usa-e2.cloudhub.io/

Colecciones Postman Incluidas en carpeta.
