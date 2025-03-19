# Arrays y documentos anidados

1. Para hacer esta práctica vamos a cargar unos datos ficticios de empresas.
2. Tienes un fichero denominado “personas.json”
```json
db.personas.insertMany([
{
    "nombre": "Daniel Espinal",
    "direccion": {
        "calle": "8389 Janie Streets",
        "ciudad": "Lue Amnat",
        "pais": "Thailand"
    },
    "colores": [
        "black",
        "green",
        "olive",
        "sky blue"
    ],
    "ingresos": 4098
},
{
    "nombre": "Ana Tirado",
    "direccion": {
        "calle": "895 Carole Forge",
        "ciudad": "Macau",
        "pais": "Macao"
    },
    "colores": [
        "sky blue",
        "azure",
        "indigo",
        "azure"
    ],
    "ingresos": 7524
},
{
    "nombre": "Laura Oquendo",
    "direccion": {
        "calle": "2800 Samir Trail",
        "ciudad": "Bijelo Polje",
        "pais": "Montenegro"
    },
    "colores": [
        "pink",
        "blue",
        "teal"
    ],
    "ingresos": 8707
},
{
    "nombre": "Laura Salcedo",
    "direccion": {
        "calle": "11046 Cayla Centers",
        "ciudad": "Rosso",
        "pais": "Mauritania"
    },
    "colores": [
        "indigo",
        "green",
        "yellow",
        "salmon"
    ],
    "ingresos": 7435
},
{
    "nombre": "Ricardo Jaime",
    "direccion": {
        "calle": "88712 Thompson Cliffs",
        "ciudad": "Prao",
        "pais": "Vietnam"
    },
    "colores": [
        "teal",
        "green"
    ],
    "ingresos": 1677
},
{
    "nombre": "Jordi Pulido",
    "direccion": {
        "calle": "90025 Bednar Spur",
        "ciudad": "Ashgabat",
        "pais": "Turkmenistan"
    },
    "colores": [
        "orange",
        "green",
        "tan"
    ],
    "ingresos": 10165
},
{
    "nombre": "Sergi Cordero",
    "direccion": {
        "calle": "0605 Delfina Lodge",
        "ciudad": "Obiozara",
        "pais": "Nigeria"
    },
    "colores": [
        "indigo",
        "sky blue",
        "red"
    ],
    "ingresos": 7134
},
{
    "nombre": "Ángel Anguiano",
    "direccion": {
        "calle": "20780 McLaughlin Union",
        "ciudad": "Paramaribo",
        "pais": "Suriname"
    },
    "colores": [
        "plum",
        "silver",
        "olive",
        "salmon",
        "silver"
    ],
    "ingresos": 5712
},
{
    "nombre": "Jordi Baeza",
    "direccion": {
        "calle": "7415 Adela Court",
        "ciudad": "‘Ohonua",
        "pais": "Tonga"
    },
    "colores": [
        "fuchsia",
        "silver"
    ],
    "ingresos": 9129
},
{
    "nombre": "Ricardo Avilés",
    "direccion": {
        "calle": "29229 Roob Points",
        "ciudad": "Macau",
        "pais": "Macao"
    },
    "colores": [
        "yellow",
        "yellow",
        "fuchsia",
        "salmon",
        "blue",
        "yellow"
    ],
    "ingresos": 7178
},
{
    "nombre": "Anni Niño",
    "direccion": {
        "calle": "207 Taylor Cliffs",
        "ciudad": "Buenaventura",
        "pais": "Colombia"
    },
    "colores": [
        "yellow",
        "salmon",
        "yellow"
    ],
    "ingresos": 7387
},
{
    "nombre": "Andrea Paredes",
    "direccion": {
        "calle": "09438 Vandervort Drives",
        "ciudad": "San Antonio",
        "pais": "Puerto Rico"
    },
    "colores": [
        "green",
        "indigo",
        "yellow",
        "salmon",
        "grey",
        "violet"
    ],
    "ingresos": 6340
},
{
    "nombre": "Manuel Leiva",
    "direccion": {
        "calle": "7008 Roob Passage",
        "ciudad": "Porto dos Mosteiros",
        "pais": "Cape Verde"
    },
    "colores": [
        "indigo",
        "plum",
        "orange"
    ],
    "ingresos": 6606
},
{
    "nombre": "Ricardo Collazo",
    "direccion": {
        "calle": "0167 Romaguera Radial",
        "ciudad": "",
        "pais": "British Indian Ocean Territory (Chagos Archipelago)"
    },
    "colores": [
        "violet",
        "sky blue",
        "sky blue",
        "olive",
        "olive",
        "silver"
    ],
    "ingresos": 3173
},
{
    "nombre": "Laura Lovato",
    "direccion": {
        "calle": "3549 Pagac Green",
        "ciudad": "Alindao",
        "pais": "Central African Republic"
    },
    "colores": [
        "magenta",
        "sky blue",
        "salmon"
    ],
    "ingresos": 7822
},
{
    "nombre": "Lorena Saiz",
    "direccion": {
        "calle": "1611 Oscar Walk",
        "ciudad": "The Pas",
        "pais": "Canada"
    },
    "colores": [
        "orchid",
        "teal",
        "pink"
    ],
    "ingresos": 10407
},
{
    "nombre": "Manuel Campos",
    "direccion": {
        "calle": "291 Waelchi Crest",
        "ciudad": "Holetown",
        "pais": "Barbados"
    },
    "colores": [
        "maroon",
        "red",
        "cyan",
        "blue",
        "white",
        "gold"
    ],
    "ingresos": 11230
},
{
    "nombre": "Salvador Meraz",
    "direccion": {
        "calle": "9327 Satterfield Alley",
        "ciudad": "Tuntange",
        "pais": "Luxembourg"
    },
    "colores": [
        "red",
        "yellow",
        "orange",
        "violet"
    ],
    "ingresos": 4058
},
{
    "nombre": "Roser Olivárez",
    "direccion": {
        "calle": "5112 Lueilwitz Expressway",
        "ciudad": "Suva",
        "pais": "Fiji"
    },
    "colores": [
        "tan",
        "black",
        "salmon",
        "purple",
        "black",
        "green"
    ],
    "ingresos": 1850
},
{
    "nombre": "Anni Saiz",
    "direccion": {
        "calle": "482 Adams Street",
        "ciudad": "",
        "pais": "British Indian Ocean Territory (Chagos Archipelago)"
    },
    "colores": [
        "green",
        "orange",
        "violet",
        "orchid",
        "tan"
    ],
    "ingresos": 10997
},
{
    "nombre": "Ángel Zaragoza",
    "direccion": {
        "calle": "2758 O'Connell Ridge",
        "ciudad": "Barclayville",
        "pais": "Liberia"
    },
    "colores": [
        "orange",
        "maroon",
        "white",
        "tan",
        "red",
        "maroon"
    ],
    "ingresos": 9869
}]);
```
3. Debes poner el resultado de las consultas en cada apartado
- Buscar las personas que vivan en Colombia
```json
db.personas.find({ "direccion.pais": "Colombia" })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cec'),
    nombre: 'Anni Niño',
    direccion: {
      calle: '207 Taylor Cliffs',
      ciudad: 'Buenaventura',
      pais: 'Colombia'
    },
    colores: [ 'yellow', 'salmon', 'yellow' ],
    ingresos: 7387
  }
]
```
-- Con proyeccion
```json
db.personas.find({ "direccion.pais": "Colombia" }, { "nombre": 1, "direccion.pais": 1 })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cec'),
    nombre: 'Anni Niño',
    direccion: { pais: 'Colombia' }
  }
]
test> db.personas.find({ "colores": "pink" })
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce4'),
    nombre: 'Laura Oquendo',
    direccion: {
      calle: '2800 Samir Trail',
      ciudad: 'Bijelo Polje',
      pais: 'Montenegro'
    },
    colores: [ 'pink', 'blue', 'teal' ],
    ingresos: 8707
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf1'),
    nombre: 'Lorena Saiz',
    direccion: { calle: '1611 Oscar Walk', ciudad: 'The Pas', pais: 'Canada' },
    colores: [ 'orchid', 'teal', 'pink' ],
    ingresos: 10407
  }
]
```

- Personas a las que le guste el color rosa
```json
db.personas.find({ "colores": "pink" })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce4'),
    nombre: 'Laura Oquendo',
    direccion: {
      calle: '2800 Samir Trail',
      ciudad: 'Bijelo Polje',
      pais: 'Montenegro'
    },
    colores: [ 'pink', 'blue', 'teal' ],
    ingresos: 8707
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf1'),
    nombre: 'Lorena Saiz',
    direccion: { calle: '1611 Oscar Walk', ciudad: 'The Pas', pais: 'Canada' },
    colores: [ 'orchid', 'teal', 'pink' ],
    ingresos: 10407
  }
]
```

-- Con Proyeccion
```json
db.personas.find({ "colores": "pink" }, { "nombre": 1, "colores": 1 })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce4'),
    nombre: 'Laura Oquendo',
    colores: [ 'pink', 'blue', 'teal' ]
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf1'),
    nombre: 'Lorena Saiz',
    colores: [ 'orchid', 'teal', 'pink' ]
  }
]
```

- Personas cuyo tercer color preferido sea el amarillo (yellow). Recuerda que los arrays comienzan por Cero. Deben salir 3
```json
db.personas.find({ "colores.2": "yellow" })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce5'),
    nombre: 'Laura Salcedo',
    direccion: {
      calle: '11046 Cayla Centers',
      ciudad: 'Rosso',
      pais: 'Mauritania'
    },
    colores: [ 'indigo', 'green', 'yellow', 'salmon' ],
    ingresos: 7435
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cec'),
    nombre: 'Anni Niño',
    direccion: {
      calle: '207 Taylor Cliffs',
      ciudad: 'Buenaventura',
      pais: 'Colombia'
    },
    colores: [ 'yellow', 'salmon', 'yellow' ],
    ingresos: 7387
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ced'),
    nombre: 'Andrea Paredes',
    direccion: {
      calle: '09438 Vandervort Drives',
      ciudad: 'San Antonio',
      pais: 'Puerto Rico'
    },
    colores: [ 'green', 'indigo', 'yellow', 'salmon', 'grey', 'violet' ],
    ingresos: 6340
  }
]
```
- Personas cuyo tercer color preferido sea el amarillo (yellow) y que vivan en Mauritania (debe salir uno)
```json
db.personas.find({ "colores.2": "yellow", "direccion.pais": "Mauritania" })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce5'),
    nombre: 'Laura Salcedo',
    direccion: {
      calle: '11046 Cayla Centers',
      ciudad: 'Rosso',
      pais: 'Mauritania'
    },
    colores: [ 'indigo', 'green', 'yellow', 'salmon' ],
    ingresos: 7435
  }
]
```

- Usando el operador $all averiguar las personas que les gusta el plata (silver) y el salmon (salmon)
```json
db.personas.find({ "colores": { $all: ["silver", "salmon"] } })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce9'),
    nombre: 'Ángel Anguiano',
    direccion: {
      calle: '20780 McLaughlin Union',
      ciudad: 'Paramaribo',
      pais: 'Suriname'
    },
    colores: [ 'plum', 'silver', 'olive', 'salmon', 'silver' ],
    ingresos: 5712
  }
]
```

- Con el operador $elemMatch, averigua las personas que les guste el rosa (Pink) o el rojo (red)
```json
db.personas.find({ "colores": { $elemMatch: { $in: ["pink", "red"] } } })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce4'),
    nombre: 'Laura Oquendo',
    direccion: {
      calle: '2800 Samir Trail',
      ciudad: 'Bijelo Polje',
      pais: 'Montenegro'
    },
    colores: [ 'pink', 'blue', 'teal' ],
    ingresos: 8707
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce8'),
    nombre: 'Sergi Cordero',
    direccion: {
      calle: '0605 Delfina Lodge',
      ciudad: 'Obiozara',
      pais: 'Nigeria'
    },
    colores: [ 'indigo', 'sky blue', 'red' ],
    ingresos: 7134
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf1'),
    nombre: 'Lorena Saiz',
    direccion: { calle: '1611 Oscar Walk', ciudad: 'The Pas', pais: 'Canada' },
    colores: [ 'orchid', 'teal', 'pink' ],
    ingresos: 10407
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf2'),
    nombre: 'Manuel Campos',
    direccion: {
      calle: '291 Waelchi Crest',
      ciudad: 'Holetown',
      pais: 'Barbados'
    },
    colores: [ 'maroon', 'red', 'cyan', 'blue', 'white', 'gold' ],
    ingresos: 11230
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf3'),
    nombre: 'Salvador Meraz',
    direccion: {
      calle: '9327 Satterfield Alley',
      ciudad: 'Tuntange',
      pais: 'Luxembourg'
    },
    colores: [ 'red', 'yellow', 'orange', 'violet' ],
    ingresos: 4058
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf6'),
    nombre: 'Ángel Zaragoza',
    direccion: {
      calle: "2758 O'Connell Ridge",
      ciudad: 'Barclayville',
      pais: 'Liberia'
    },
    colores: [ 'orange', 'maroon', 'white', 'tan', 'red', 'maroon' ],
    ingresos: 9869
  }
]
```

-- Con una proyeccion
```json
db.personas.find({ "colores": { $elemMatch: { $in: ["pink", "red"] } } }, 
{ "nombre": 1, "colores":1 })
```
-Resultado
```json
[
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce4'),
    nombre: 'Laura Oquendo',
    colores: [ 'pink', 'blue', 'teal' ]
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0ce8'),
    nombre: 'Sergi Cordero',
    colores: [ 'indigo', 'sky blue', 'red' ]
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf1'),
    nombre: 'Lorena Saiz',
    colores: [ 'orchid', 'teal', 'pink' ]
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf2'),
    nombre: 'Manuel Campos',
    colores: [ 'maroon', 'red', 'cyan', 'blue', 'white', 'gold' ]
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf3'),
    nombre: 'Salvador Meraz',
    colores: [ 'red', 'yellow', 'orange', 'violet' ]
  },
  {
    _id: ObjectId('67da1cfa3feac52e1dcb0cf6'),
    nombre: 'Ángel Zaragoza',
    colores: [ 'orange', 'maroon', 'white', 'tan', 'red', 'maroon' ]
  }
]
```