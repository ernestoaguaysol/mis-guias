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
