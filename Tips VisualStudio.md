# Tips Visual Studio

## Atajos de teclado Windows

| Comando      | Descrición |
| ---          | ---        |
| Ctrl + h     | Cambia todo lo que indiques por otra palabra |
| Ctrl + k + s | Nos da la posibilidad de elegir distintas opciones. la que mas uso personalmemte es #Region|

## Sintaxis

* Agregar @ (arroba) adelante mata cualquier palabra reservada  

## DataNotation

* Podemos recibir un objeto *Json* de una manera pero tratarla de otra manera dentro de nuestro código. Por ejemplo:
~~~ C#
  [Json Property(PropertyName="disclamer")]
  public string Disclamer{ get; }{ set; }
~~~

En el siguiente ejemplo vemos que la recibo como "diclamer" empezando con minuscula y la trato como **Disclamer** 
empezando con mayúscula. Notar que la diferencia solo es de mayúscula y minúscula pero la puedo llamar de distinta manera, pero hay que tener en cuenta que para un mejor entendimiento del código hay que hacer la menor cantidad de cambios posibles, pero la razón del cambio se debe a que es una buena práctica de programación que una propiedad píblica empieze con la letra Mayuscula.
