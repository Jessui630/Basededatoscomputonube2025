# Crud y consultas en MongoDB
## Crear base de datos
Solo se crea si contiene por lo menos una coleccion


#Como crear una coleccion 

** use bd1 **




```json
db.alumnos.insertOne(
{
nombre:'Soyla',
apellido1: 'Vaca',
edad:32,
ciudad: 'San Miguel de las Piedras'
})
```



## Comsulta toda la tabla

db.alumnos.find({})


## Insersion de un documento mas complejo con array

```json
db.alumnos.insertOne(
 {
 nombre: "Joaquin",
 apellido: "Dorian",
 apellido2: "Guerrero",
 edad: 15,
 aficiones: [
              'Cerveza', 'Hueva', "Cannabis"
            ]
 })
```


 
 ## Insersion de documentos mas complejos con documentos anidados y Id


```json
db.alumnos.insertOne(
 {
 nombre: "Jose Luis",
 apellido: 'Ortiz',
 edad: 45,
 estudios: [
            "Ing en Sistemas Computacionales",
            "Maestria en Tecnologias de la Informacion"
          ],
 experiencia: {
               lenguaje: 'Sql',
               sdb:"SQL Server",
               aniosExp: 14
             }
 })
```

```json
 db.alumnos.insertOne(
 {
    _id: 3,
    nombre:'Sergio',
    apellido: 'Ramos',
    equipo: 'Monterrey',
    aficiones: ['Dinero', 'Hombres', 'Fiesta'],
    talentos: {
            futbol: true,
            bañarse: false
    }
 })
```


## Insertar multiples documentos 

```json
db.alumnos.insertMany(
 [
   {
     _id: 12,
     nombre: 'Roberto',
     apellido: 'Gomez',
     edad: "23",
     descripcion: "Es un comediante bueno"
 },
 {
   nombre: "Luis",
   apellido: "Suarez",
   edad: 43,
   habilidades: [
                  'Correr', 'dormir', 'morder'
                ],
    direcciones: {
                calle: 'Del infierno',
                numero: 666
              },
    esposas: [
            {
                nombre: "Marisol",
                edad: 20,
                pension: 350,
                hijos:['Joaquin', 'Bridget']
            },
            {
                nombre: "Dorien",
                edad: 46,
                pension: 6500.56,
                complaciente: true
            }
    ]
 }
 ]
 )
```


# Practica 1

## Cargar datos

```json
[Libros.json](./data/libros.json)
```

## Busquedas. Condiciones simples de igualdad. Metodo find()

1. Seleccionar todos los documentos de la coleccion libros

```json
 db.libros.find({})
```

2. Mostrar todos los documentos que sean de la editorial biblio

```json
db.libros.find({editorial: 'Biblio'})
```

3. Mostrar todos los documentos que el precio sea 25

```json
db.libros.find({precio: 25})
```

4. Seleccionar todos los documentos donde el titulo sea Json para todos

```json
db.libros.find({titulo: 'JSON para todos'})
```


## Operadores de comparacion

```json
[Operadores de comparacion](https://www.mongodb.com/docs/manual/reference/operator/query/)

![Operadores de comparacion](./img/operadores_relacionales.png)
```

1. Mostrar todos los documentos donde el precio sea mayor a 25

```json
db.libros.find({precio:{$gt: 25}})
```

2. Mostrar los documentos donde el precio sea 25

```json
db.libros.find(
 {
   precio:{$eq: 25}
 }
)
```

3. Mostrar los documentos cuya cantidad sea menor a 5

```json
db.libros.find({precio:{$lt: 5}})
```

4. Mostrar los documentos que pertenezcan a la editorial biblio o planeta

```json
db.libros.find({editorial:{$in: ['Biblio', 'Planeta']}})
```

5. Mostrar todos los documentos de libross que cuestes 20 o 25

```json
db.libros.find({precio:{$in:[20, 25]}})
```

6. Mostrar todos los documentos de libros que no cuesten 20 o 25

```json
db.libros.find({precio:{$nin:[20, 25]}})
```

7. Mostrar el primer documento de libros que cueste 20 o 25

```json
db.libros.findOne({precio:{$in:[20, 25]}})
```

## Operadores logicos 

```json

[Operadores logicos](https://www.mongodb.com/docs/manual/reference/operator/query/)

![Operadores logicos](./img/operadores_logicos.png)
```

### Operador AND

Dos posibles opciones de AND 

1. La simple mediante condiciones separadas por comas

Sintaxis
<br> 
db.coleccion.find({condicion1, condicion2}) -> Con esto asume que es una *and*

2. Usando el operador $and

*Sintaxis*<br>

```json
db.coleccion.find(
 {
   $and:[{condicion1},
   {condicion2}]
 }
)
```

### Ejercicios

1. Mostrar todos aquellos libros que cuesten mas de 25 y cuya cantidad sea inferior a 15

*Forma simple*

```json
db.libros.find(
 {  
   precio: { $gt: 25 },  
   cantidad: { $lt: 15 }
 } 
)
```

2. Mostrar todos aquellos libros que cuesten mas de 25 y cuya cantidad sea inferior a 15 y id igual 4

```json
db.libros.find(
 {  
      precio: { $gt: 25 },  
      cantidad: { $lt: 15 }, 
      _id: {$eq: 4} 
 } 
)
```

*Operador $and*

1. Mostrar todos aquellos libros que cuesten mas de 25 y cuya cantidad sea inferior a 15

```json
db.libros.find( 
 {
    $and: [{precio: {$gt: 25}},
    {cantidad: {$lt: 15}}]
 }
)
```

2. Mostrar todos aquellos libros que cuesten mas de 25 y cuya cantidad sea inferior a 15 y id igual 4

```json
db.libros.find( 
 {
    $and: [{precio: {$gt: 25}},
    {cantidad: {$lt: 15}},
    {_id: {$eq: 4}}]
 }
)
```

### Operador OR

#### Mostrartodos aquellos libros que cuesten mas de 25 o cuya cantidad sea inferiora 15

```json
db.libros.find( 
 {
    $or: [{precio: {$gt: 25}},
    {cantidad: {$lt: 15}}]
 }
)
```

### AND y OR Combinadas

1. Mostrar los libros de la editorial Biblio con precio mayor a 40 o libros de la editorial Planeta
con precio mayor a 30

```json
db.libros.find(
   {
     $or : [
       {$and:[{editorial: 'Biblio'},{precio:{$gt: 30}}]},
       {$and: [{editorial:{$eq:'Planeta'}},{precio:{$gt:20}}]}
           ] 
})
```

## Proyeccion de Columnas

*** Sintaxis ***

db.coleccion.find(filtro, columnas)

db.libros.find({},{titulo:1})

1. Seleccionar todos los documentos, mostrando el titulo y la editorial

```json
db.libros.find({},{titulo:1, editorial:1})
```

2. Seleccionar todos los documentos de la editorial planeta, mostrando 
solamente el titulo y la editorial

```json
db.libros.find({editorial: 'Planeta'}, {_id:0,titulo:1 ,editorial:1})
```

## Operador exists (Permite saber si un campo si un campo se encuentra o no en un documento)

```json
db.libros.find( { editorial:{ $exists:true } } )
```

1. Mostrar todos los documentos que no contengan el campo cantidad

```json
db.libros.find(
 {
   cantidad:{$exists:false}
 }
)
```

## Operador Type (Permite preguntar si un determinado campo corresponde con un tipo) 

[Operador Type](https://www.mongodb.com/docs/manual/reference/operator/query/type/#mongodb-query-op.-type)

1. Mostrar todos los documentos donde el precio sean dobles

```json
db.libros.find({precio:{$type:1}})
db.libros.find({precio:{$type:16}})
```

```json
db.libros.insertOne({
  _id:11,
  titulo: 'IA',
  editorial: 'Terra', 
  precio:125.4,
  cantidad: 20
})
```

```json
db.libros.insertMany([
 {
    _id: 12,
    titulo: 'IA',
    editorial: 'Terra',
    precio: 125, 
	cantidad: 20
  },
  {
    _id: 13,
    titulo: 'Python para todos',
    editorial: 2001,
    precio: 200, 
	cantidad: 30
  }]
  )
```

```json
db.libros.find({_id:13}

db.libros.insertOne({editorial:{$type:16}})
```

1. Seleccionar todos los documentos don


## Practica de consultas
1. Instalar las tools de monofdb


2. Cargar json
--En local:
  mongoimport --db curso --collection empleados --file empleados

# Modificando Documentos
## Comandos importabtes
1. updateOne -> Modififcar un solo documento
2. updateMany -> Modificar multiples documentos 
3. replaceOne -> Sustituir el contenido completo de un documento

Tiene el segundo formato:

```json
db.collection.updateOne(
  {filtro},{operador: }
)
```

### Operador set
1. Modificar un documento
```json
db.libros.updateOne({titulo:'Python para torpes'},{$set:{titulo:'Java para todos'}})
```

2. Actualizar el precio a 100 y la cantidad a 50 para el _id: 10
```json
db.libros.updateOne({_id:10},{$set:{precio:100, cantidad: 50}})
```

### Modificar Multiples Documentos

--Modificar todos los documentos donde el precio sea mayor a 100 a un precio de 150
```json
db.libros.updateMany({precio:{$gt:100}},{$set:{precio:150}})
```

2. Operador $inc y $mul
-Actualizar con multiplicaciones de 2 todos los documentos mayores a 20
```json
db.libros.updateMany({cantidad:{$gt:20},{$mul:{cantidad:2}}})
```

--Actualizar todos los documentos donde el precio sea mayor a 20 y
se multiplique por 2 la cantidad y el precio

```json
db.libros.updateMany({precio:{$gt:20}},{$mul:{cantidad:2, precio:2}})
```

3. Remplazar Documentos (replaceOne)
```json
db.libros.updateOne({_id:2},{$set:{precio:56,existencia:10}})

db.libros.replaceOne({_id:2}, {titulo:'De la Tierra a la Luna', autor: 'Julio Verne', precio: 20})
```

## Borrar Documentos

1. deleteOne -> Elimina un solo documento 
2. deleteMany -> Elimina varios documentos

1. Eliminar el documento con ID 2
```json
db.libros.deleteOne({_id:2})
```

2. Eliminar los documentos donde la cantidad sea mayor o igual a 100
```json
db.libros.deleteMany({cantidad:{$gte:100}})
```

# Expresiones Regulares

1. Buscar los libros que contenga el titulo la letra t 
```json
db.libros.find({titulo:/t/})
```

2. Buscar los libros que en el titulo contenganla palabra json
```json
db.libros.find({titulo:/JSON/})
```

3. Buscar todos los documentos que en el titulo terminen en tos
```json
db.libros.find({titulo:/tos$/})
```

4. Todos los documentosque en el titulo comiencen con J 
```json
db.libros.find({titulo:/^J/})
```

# Operador $regex
[Operador regex](Enlace Aqui...)

-- Seleccionar los libros que contengan la palabra 'para' en titulo
```json
db.libros.find({titulo:{$regex: 'para'}})

db.libros.find({titulo:{$regex: 'JSON'}})

db.libros.find({titulo:{$regex:/JSON/}})
```
-Distingue entre mayusculas y minusculas

```json
db.libros.find({titulo:{$regex:/json/}}) 

No disitingue entre mayusculas y minusculas

db.libros.find({titulo:{$regex:/json/, $options: "j"}}) ->| Distingue entre mayusculas y minusculas

db.libros.find({titulo:{$regex:/json/i}})

```

-- Seleccionar todos los libros que comiencen con j o J
```json
db.libros.find({titulo:{$regex:/j/i}})
```

-- Seleccionar todos los libros que terminen en 'es'
```json
db.libros.find({titulo:{$regex:/es$/i}})

db.libros.find({titulo:{$regex:'es$',options:'i'}})
```

# Metodo sort (Ordenar Documentos)

1. Ordenar los libros de manera ascendente por el precio
```json
db.libros.find({},{titulo:1, precio:1, _id:0}).sort({precio:1})
```

2. Ordenar los libros de manera descendente por el precio
```json
db.libros.find({},{titulo:1, precio:1, _id:0}).sort({precio:-1})
```

3. Ordenar los libros de manera ascendente por la editorial y de manera descendente por el precio,
mostrando el titulo, el precio y la editorial
```json
db.libros.find({},{titulo:1, precio:1, editorial:1, _id:0}).sort({editorial:1,precio:-1})
```

# Otros Metodos skip, limit, size
```json
db.libros.find({}, {titulo:1, precio:1, _id:0, editorial:1}).size()

db.libros.find({}).size()

db.libros.find({titulo:{$regex:/java/i}}).size()
```

-- Buscar todos los libros pero mostrando los dos primeros
```json
db.libros.find({},{titulo:1, editorial:1, precio:1, _id:0}).limit(2)
```

-- Mostrar los 3 ultimos libros
```json
db.libros.find({},{titulo:1, precio:1, editorial:1, _id:0}).sort({precio:-1}).limit(3)
```

--

```json
db.libros.find({},{titulo:1, precio:1, editorial:1}).skip(2)
```

-- Seleccionar todos los libros ordenados por titulo de forma descendente saltando los 
2 primeros documentos y que muestre el tamaño

```json 
db.libros.find({}).sort({titulo:-1}).skip(2).size()
```

# Borrar colecciones y bases de datos
db.createCollection('ejemplo')

show collections

db.ejemplo.insertOne({nombre:''Chapuin})

db.ejemplo.drop()

db.dropDatabase()

```json

```