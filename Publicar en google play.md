# Publicar en Google Play

## Icono de la app

* Vamos a usar los siguientes enlaces para el **Icono de la app**:  
https://romannurik.github.io/AndroidAssetStudio/  
https://www.iconfinder.com/

> si lo quieres hacer desde cero aqui hay mas referencias  
https://material.io/guidelines/style/icons.html#

* Ahora seguimos las instrucciones de xamarin  
https://developer.xamarin.com/guides/android/deployment,_testing,_and_metrics/publishing_an_application/part_1_-_preparing_an_application_for_release/

Para una visión rápida vamos  a hacer los siguientes pasos para la **Preparación del apk**:  

1- Agregar todos los iconos generados en el proyecto **Android** en la ruta **Resources/drawable** y sus derivados (drawable-hdpi, drawable-xhdpi, drawable-xxhdpi)  

2- Cambiar el mapeo del icono por defecto que se encuentra en MainActivity.cs en la siguiente linea de código:  
``[Activity(Label = "Calculadora", Icon = "@drawable/icon", Theme = "@style/MainTheme", MainLauncher = true, ConfigurationChanges = ConfigChanges.ScreenSize | ConfigChanges.Orientation)]``  
cambiar ``Icon = "@drawable/icon"`` del dice **icon** por el nombre del icono que queremos por ejemplo ``Icon = "@drawable/ic_calc"``  
luego provamos que se vea el icono.

> Nota: los nombres no llevan extención.

3- Doble click en **properties** y en la pestaña **Android Manifest** cambiamos las siguientes propiedades:

![](https://github.com/ernestoaguaysol/mis-guias/blob/master/Imagenes/Calculadora/calculadora-Captura%20de%20pantalla%20(30).png)

> Nota: el nombre del paquete es recomendable seguir eo estandar com.nombre.nombreapp

4- en la pestaña **Android Options** deshabilitar las siguientes propiedades:

![](https://github.com/ernestoaguaysol/mis-guias/blob/master/Imagenes/Calculadora/calculadora-Captura%20de%20pantalla%20(31).png)

5- Ahora hacemos click con el segundo botón en el proyecto **Android** y hacemos click en **Archive** y si todo va bien nos debe generar el paquete y nos mustra una imagen como ésta:

![](https://github.com/ernestoaguaysol/mis-guias/blob/master/Imagenes/Calculadora/calculadora-Captura%20de%20pantalla%20(32).png)

le damos click en **Distribute** y luego en **Ad Hoc** para alojarlo localmente.

6- El siguiente paso es generar un sertificado o utilizar uno existente **ES MUY IMPORTANTE GUARDAR EL PASSWORD EN UN LUGAR A SALVO**.  
Si creamos un nuevo certificado hay que rellenar todos los campos por ejemplo:
![](https://github.com/ernestoaguaysol/mis-guias/blob/master/Imagenes/Calculadora/calculadora-Captura%20de%20pantalla%20(33).png)

Guardamos y nos va a pedir donde lo vamos a guardar, luego aceptamos todo y lo va a generar.

## Cuenta en Goople Play Developer

* Vamos al siguiente enlace https://play.google.com/apps/publish/ y seguimos todos los pasos

> si no te direcciona el enlace "Goooglea" :)

> La cuenta necesitaremos nuestra tarjeta de crédito, en google play cuesta $30 dolares de por vida a comparación de Apple que cuesta $99 dolares.


## Preparetivos para el lanzamiento de la App

>A tener en cuenta:  
*"Las imagenes alojadas no pueden contener derechos de autor, por ejemplo nunca debes poner una imagen de un famoso o escudo de futbol que esté con derechos de autor aunque hay casos que te permita, es mejor evitarlos"*.  

* Una vez creada la cuenta vamos a **Crear una Aplicación**, lugo ponemos el titulo y aceptamos.

* Lo siguiente es rellenar los campos de **Ficha de Play Store**, para una rapida publicación solo rellenar los campos obligatorios. Tener en cuenta las medidas de las imagenes.  
> Nota: "Es fundamental colocar una url en **politicas de privacidad**"  
> Para llenar la **Calificación de contenido** primero debenos subir el apk.  

* Para subir apk vamos a **versiones de la app** y luego a **ADMINISTRAR VERSIÓN DE PRODUCCIÓN**, luego creamos la versión y subimos el apk desde la biblioteca donde lo tenemos guardado.

Luego de rellenar los campos de **Novedades de este lanzamiento** de damos a **guardar** y luego **revisar**.

* Antes de **Revisión y lanzamiento** tenemos que ir a **Calificación de contenido**, llenamos y respondemos todos los campos necesarios.  
Luego de contestar todo aceptamos y solicitamos la calificación.

* Ahora vamos a **Precios y distribución** contestamos los campos requeridos, como consejo hacer la app gratis, que sea para todo el mundo y no olvidar de marcar los dos últimos campos que son obligatorios.

### Listos para Publicar  
* Para publicar tiene que estar todas las palomitas en verde, y tiene que aparecer **Listos para publicar** como la siguiente imagen:  
![](https://github.com/ernestoaguaysol/mis-guias/blob/master/Imagenes/Calculadora/calculadora-Captura%20de%20pantalla%20(34).png)

> Si no llegara a salir ese mensaje en la parte donde dice **Listos para publicar** aparecerá otro recuadro con la frase **¿Por que no puedo publicar?** y nos fijamos el motivo.

* Guardamos borrador y hacemos click en **Listos para publicar**, luego a **administrar lanzamiento**. luego vamos a **administrar versión de producción**, **Editar Versión**, **Revisar**, y por último **INICIAR LANZAMIENTO DE VERSIÓN EN PRODUCCIÓN** y **Confirmar**.  Ahora quedará un recuadro con la publicación pendiente... Ahora todo queda en manos de Google para que nos confirme la publicación.  

![](https://github.com/ernestoaguaysol/mis-guias/blob/master/Imagenes/Calculadora/calculadora-Captura%20de%20pantalla%20(35).png)

> A veces se demoran mucho, a veces no. Todo depende de San Google...  
Buena Suerte!!!
