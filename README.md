# Práctica 10
Rebeca Moreno González

## Objetivo

Comprender qué son las bases de datos NoSQL, por qué surgieron y cuáles son sus principales diferencias respecto al modelo relacional. También conocer sus ventajas y desventajas mediante el uso de un sistema NoSQL para almacenar y consultar información semiestructurada.

## Decisiones

Durante esta práctica utilicé MongoDB y MongoDB Compass para trabajar con una base de datos NoSQL documental. Primero creé una base de datos llamada **tienda** y dentro de ella una colección llamada **productos**, donde guardé información de diferentes artículos tecnológicos. Para representar cada producto utilicé documentos JSON con datos como el nombre, el precio y un apartado de características donde se almacena información más específica.

También quise comprobar la flexibilidad que ofrece MongoDB al trabajar con su estructura de documentos. Para esto agregué un producto que incluía un campo extra llamado **marca**, aunque los demás documentos no contaban con ese atributo. De esta manera pude observar que no es necesario modificar la estructura de toda la colección cuando se quiere agregar información nueva.

Después realicé diferentes consultas para buscar productos según ciertas condiciones, como su rango de precios o algunas características específicas. También hice búsquedas dentro de los subdocumentos para encontrar productos según su memoria RAM y color. Por último, comparé MongoDB con un sistema gestor de bases de datos relacional, tomando en cuenta su consistencia, escalabilidad y facilidad de modelado.

## Pruebas realizadas

### Para la actividad:

1. Creé una base de datos llamada **tienda** y una colección llamada **productos** desde MongoDB Compass.
2. Inserté diferentes documentos JSON con información de varios productos tecnológicos.
3. Organicé algunos datos utilizando subdocumentos dentro del campo **caracteristicas**.
4. Añadí un producto con un campo extra llamado **marca** para comprobar que se pueden manejar diferentes estructuras dentro de una misma colección.
5. Consulté todos los documentos para revisar que los productos se hubieran guardado correctamente.
6. Realicé búsquedas utilizando operadores de comparación para encontrar productos dentro de ciertos rangos de precios.
7. Probé consultas sobre datos específicos de los subdocumentos, como la memoria RAM y el color.
8. Revisé los resultados de cada consulta para asegurarme de que coincidieran con los datos almacenados.

## Errores

Al comenzar la práctica tuve algunos problemas para conectarme a MongoDB Compass. Cuando intenté utilizar la dirección que aparece por defecto, me encontré con el siguiente error:

```text
connect ECONNREFUSED 127.0.0.1:27017
```
Esto sucedió porque el servidor de MongoDB no estaba instalado o iniciado correctamente en mi equipo. Para resolverlo tuve que instalar MongoDB Community Server y asegurarme de que el servicio estuviera funcionando antes de volver a intentar la conexión desde Compass.

También tuve problemas durante la instalación, ya que apareció un error relacionado con Windows Installer que no me permitía continuar con el proceso. Después de revisar y probar algunas soluciones, finalmente pude completar la instalación y utilizar MongoDB sin problemas.

## Conclusión
En esta práctica aprendí a trabajar con MongoDB y a entender mejor cómo funcionan las bases de datos NoSQL documentales. Pude practicar la creación de bases de datos y colecciones, insertar documentos JSON, utilizar subdocumentos y realizar consultas para encontrar información específica.

También me sirvió comparar ambos tipos de sistemas, ya que pude conocer mejor sus ventajas y en qué situaciones conviene utilizar cada uno. Considero que esta práctica me ayudó a ampliar mis conocimientos sobre las diferentes formas de almacenar y administrar información.
