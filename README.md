<h1>Proyecto Api Market</h1>

### Caracteristicas

- API de supermercado online;
- Desarrollada en java con Framework Spring;
- Cuenta con seguridad jwt por lo que debera generar token para interactuar;
- Version de Java utilizada 8 ;
- Version de Spring 2.5.5 ;
- implementaciones: MapStruct version 1.5.3:
   con esto evitamos que el proyecto se acople a una base de datos puntual Es decir si en un futuro se cambia la base de datos.  Incluso si se la cambia por una que no sea SQL, que por ejemplo se cambie a Mongo donde hay collecciones y eso haria que la api tenga que cambiar completamente. Por eso al implementar MapStruct nos evitamos esto simplemente creando un nuevo mapper y el codigo seguira funcionando exactamente igual sin tener que modificarlo.
 <h4>DOCUMENTACION</h4>
- implementaciones: Swagger version 3.0.0
-  Swagger ui para visualizacion  version 3.0.0




## Editor utilizado netbeans version 15

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/v1669881926/Api-market/descarga_vjhdef.png)



<h1>Demostracion de las peticiones en entorno local</h1>



<h2>GET: obtener todos los productos  (Sin Autenticación )</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/v1669878566/Api-market/obtener_todas_las_compras_sin_token_efapox.png)

> Se deniega la peticion porque no esta autenticado. Error 403

#

<h2>GET: obtener todas las compras  (Ya Con Autenticación ).</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/w_1000,ar_16:9,c_fill,g_auto,e_sharpen/v1669878567/Api-market/Obtener_todas_las_compras_l724lc.png)

> Utilizando el Token accede a las peticiones. Status 200
#

<h2>GET: obtener todas las compras de un usuario  (Con Autenticación ).</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/w_1000,ar_16:9,c_fill,g_auto,e_sharpen/v1669878566/Api-market/Obtener_compras_de_un_cliente_xyrvwk.png)

> Se obtienen  las compras de un usuario atraves de su ID.
#

<h2>GET: obtener todas las compras de un usuario  (SIN Autenticación ).</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/w_1000,ar_16:9,c_fill,g_auto,e_sharpen/v1669878566/Api-market/Obtener_compras_del_cliente_denegada_rht7pa.png)

> Se rechaza la solicitud por no estar autenticado. Error 403 no tienes perimisos

#

<h2>POST: Autenticacion usando Usuario y Contraseña</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/w_1000,ar_16:9,c_fill,g_auto,e_sharpen/v1669878566/Api-market/loguearse_laond3.png)

> Se loguea y recibe el Jason Web Token
 

<h2>JASON WEB TOKEN:  donde debe colocarse el token</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/w_1000,ar_16:9,c_fill,g_auto,e_sharpen/v1669878566/Api-market/mostrar_como_usar_el_token_y7awi9.png)

> En Header se agrega una KEY = Authorization y en el VALUE = Bearer +espacio+ se pega el Token que se obtuvo al loguearse en el paso anterior. Ejemplo: "Bearer eynasdjnasjcuc638f4fhv" sin comillas.

<h2>EJEMPLO DE AUTENTICACION YA EN AMBIENTE DE PRODUCCION
SE UTILIZO AZURE PARA EL DESPLIEGUE DE LA API</h2>


<h2POST  autenticacion usando la url de produccion</h2>

![](https://res.cloudinary.com/dkm0hdlgz/image/upload/w_1000,ar_16:9,c_fill,g_auto,e_sharpen/v1669878567/Api-market/Prueba_desde_deploy_Azure_ejwhzi.png)

> Se obtiene el Token utilizando la url Azure.

-
-
-
<h2>Agregaciones importantes</h2>
-La api cuenta tambien con las posibilidades de VER AGREGAR MODIFICAR Y ELIMINAR los productos del supermercado
-Se puede Realizar compras con un usuario donde elegiras los productos que quieras luego poder ver todas las compras de cada usuario como se vio anteriormente.

<p>Si tiene interes por probar todas las caracteristicas de este proyecto puede comunicarse para facilitarle la coleccion de peticiones de Postman para que interactue libremente con la Api.</p>
-
-
<h2>¡Despedida!</h2>
<p>Este proyecto me brindó la oportunidad de aprender y utilizar nuevas tecnologías, en este caso "MAPSTRUCT" Fue mi primera vez usando esta herramienta y estoy impresionado por su eficacia en la conversión de objetos. Aprendí cómo utilizar MapStruct para mapear entidades de la base de datos a objetos de la aplicación y viceversa de manera sencilla y eficiente. Esta experiencia ha mejorado mis habilidades en el desarrollo de aplicaciones y estoy emocionado de seguir utilizando MapStruct en proyectos futuros..</p>
<p>"Por otro lado quiero agradecer por tomarse el tiempo de revisar mi proyecto. Espero que les haya gustado y encontrado útil. Si tienen alguna pregunta o sugerencia, no duden en contactarme. ¡Gracias nuevamente por su tiempo y apoyo!"</p>

<p>Author: Diego Villan </p>


