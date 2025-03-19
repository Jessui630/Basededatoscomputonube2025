# Agregaciones

1. Para hacer esta práctica vamos a cargar unos datos ficticios de empresas.
2. Tienes un fichero denominado “productos.json”
```json
db.prductos.insertMany([
{
    "codigo": 0,
    "nombre": "Fantastic Wooden Fish",
    "unidades": 95,
    "precio": 291,
    "fabricante": "Kimberly-Clark",
    "tipo": "avanzado"
},
{
    "codigo": 1,
    "nombre": "Rustic Concrete Pants",
    "unidades": 66,
    "precio": 279,
    "fabricante": "Mercury General",
    "tipo": "medio"
},
{
    "codigo": 2,
    "nombre": "Small Soft Fish",
    "unidades": 96,
    "precio": 189,
    "fabricante": "Primoris Services",
    "tipo": "medio"
},
{
    "codigo": 3,
    "nombre": "Practical Soft Pants",
    "unidades": 41,
    "precio": 67,
    "fabricante": "Hyatt Hotels",
    "tipo": "avanzado"
},
{
    "codigo": 4,
    "nombre": "Ergonomic Metal Ball",
    "unidades": 5,
    "precio": 246,
    "fabricante": "Seaboard",
    "tipo": "medio"
},
{
    "codigo": 5,
    "nombre": "Small Steel Gloves",
    "unidades": 45,
    "precio": 37,
    "fabricante": "TrueBlue",
    "tipo": "avanzado"
},
{
    "codigo": 6,
    "nombre": "Ergonomic Wooden Shirt",
    "unidades": 63,
    "precio": 238,
    "fabricante": "Securian Financial Group",
    "tipo": "avanzado"
},
{
    "codigo": 7,
    "nombre": "Handmade Steel Chair",
    "unidades": 16,
    "precio": 337,
    "fabricante": "CIT Group",
    "tipo": "medio"
},
{
    "codigo": 8,
    "nombre": "Handcrafted Soft Gloves",
    "unidades": 16,
    "precio": 282,
    "fabricante": "Pep Boys-Mann",
    "tipo": "basico"
},
{
    "codigo": 9,
    "nombre": "Fantastic Concrete Salad",
    "unidades": 49,
    "precio": 265,
    "fabricante": "Kar Auction Services",
    "tipo": "basico"
},
{
    "codigo": 10,
    "nombre": "Handmade Plastic Hat",
    "unidades": 7,
    "precio": 253,
    "fabricante": "Dick's Sporting Goods",
    "tipo": "medio"
},
{
    "codigo": 11,
    "nombre": "Refined Wooden Tuna",
    "unidades": 40,
    "precio": 212,
    "fabricante": "WGL Holdings",
    "tipo": "avanzado"
},
{
    "codigo": 12,
    "nombre": "Refined Concrete Salad",
    "unidades": 90,
    "precio": 129,
    "fabricante": "Universal Health Services",
    "tipo": "avanzado"
},
{
    "codigo": 13,
    "nombre": "Unbranded Soft Fish",
    "unidades": 53,
    "precio": 178,
    "fabricante": "Total System Services",
    "tipo": "basico"
},
{
    "codigo": 14,
    "nombre": "Small Concrete Fish",
    "unidades": 40,
    "precio": 126,
    "fabricante": "Precision Castparts",
    "tipo": "medio"
},
{
    "codigo": 15,
    "nombre": "Refined Concrete Bike",
    "unidades": 15,
    "precio": 180,
    "fabricante": "Trinity Industries",
    "tipo": "basico"
},
{
    "codigo": 16,
    "nombre": "Tasty Cotton Pants",
    "unidades": 68,
    "precio": 52,
    "fabricante": "Cabot",
    "tipo": "basico"
},
{
    "codigo": 17,
    "nombre": "Incredible Granite Gloves",
    "unidades": 71,
    "precio": 290,
    "fabricante": "Oneok",
    "tipo": "avanzado"
},
{
    "codigo": 18,
    "nombre": "Practical Metal Mouse",
    "unidades": 35,
    "precio": 190,
    "fabricante": "National Oilwell Varco",
    "tipo": "basico"
},
{
    "codigo": 19,
    "nombre": "Handcrafted Steel Chicken",
    "unidades": 55,
    "precio": 113,
    "fabricante": "State Street Corp.",
    "tipo": "medio"
},
{
    "codigo": 20,
    "nombre": "Ergonomic Metal Table",
    "unidades": 0,
    "precio": 94,
    "fabricante": "Kelly Services",
    "tipo": "avanzado"
},
{
    "codigo": 21,
    "nombre": "Tasty Wooden Ball",
    "unidades": 18,
    "precio": 76,
    "fabricante": "State Farm Insurance Cos.",
    "tipo": "basico"
},
{
    "codigo": 22,
    "nombre": "Unbranded Soft Table",
    "unidades": 41,
    "precio": 284,
    "fabricante": "Motorola Solutions",
    "tipo": "avanzado"
},
{
    "codigo": 23,
    "nombre": "Handcrafted Metal Tuna",
    "unidades": 63,
    "precio": 320,
    "fabricante": "Williams-Sonoma",
    "tipo": "medio"
},
{
    "codigo": 24,
    "nombre": "Incredible Frozen Shirt",
    "unidades": 37,
    "precio": 173,
    "fabricante": "Hawaiian Holdings",
    "tipo": "basico"
},
{
    "codigo": 25,
    "nombre": "Licensed Fresh Chicken",
    "unidades": 65,
    "precio": 233,
    "fabricante": "Kemper",
    "tipo": "basico"
},
{
    "codigo": 26,
    "nombre": "Intelligent Plastic Bike",
    "unidades": 39,
    "precio": 241,
    "fabricante": "Tractor Supply",
    "tipo": "medio"
},
{
    "codigo": 27,
    "nombre": "Sleek Steel Chicken",
    "unidades": 47,
    "precio": 131,
    "fabricante": "Mondelez International",
    "tipo": "avanzado"
},
{
    "codigo": 28,
    "nombre": "Handcrafted Granite Cheese",
    "unidades": 27,
    "precio": 304,
    "fabricante": "Lennar",
    "tipo": "medio"
},
{
    "codigo": 29,
    "nombre": "Unbranded Soft Computer",
    "unidades": 33,
    "precio": 69,
    "fabricante": "Delta Tucker Holdings",
    "tipo": "medio"
},
{
    "codigo": 30,
    "nombre": "Small Rubber Pants",
    "unidades": 89,
    "precio": 16,
    "fabricante": "Hanesbrands",
    "tipo": "basico"
},
{
    "codigo": 31,
    "nombre": "Generic Fresh Keyboard",
    "unidades": 69,
    "precio": 16,
    "fabricante": "WestRock",
    "tipo": "medio"
},
{
    "codigo": 32,
    "nombre": "Sleek Soft Towels",
    "unidades": 68,
    "precio": 68,
    "fabricante": "Alere",
    "tipo": "medio"
},
{
    "codigo": 33,
    "nombre": "Generic Concrete Hat",
    "unidades": 82,
    "precio": 70,
    "fabricante": "American Tire Distributors Holdings",
    "tipo": "basico"
},
{
    "codigo": 34,
    "nombre": "Practical Cotton Keyboard",
    "unidades": 43,
    "precio": 25,
    "fabricante": "AutoNation",
    "tipo": "medio"
},
{
    "codigo": 35,
    "nombre": "Sleek Frozen Hat",
    "unidades": 40,
    "precio": 110,
    "fabricante": "Pool",
    "tipo": "basico"
},
{
    "codigo": 36,
    "nombre": "Rustic Soft Table",
    "unidades": 73,
    "precio": 331,
    "fabricante": "Werner Enterprises",
    "tipo": "medio"
},
{
    "codigo": 37,
    "nombre": "Awesome Soft Gloves",
    "unidades": 35,
    "precio": 18,
    "fabricante": "Anthem",
    "tipo": "avanzado"
},
{
    "codigo": 38,
    "nombre": "Rustic Steel Shoes",
    "unidades": 39,
    "precio": 257,
    "fabricante": "Universal American",
    "tipo": "basico"
},
{
    "codigo": 39,
    "nombre": "Handmade Soft Chips",
    "unidades": 56,
    "precio": 208,
    "fabricante": "State Farm Insurance Cos.",
    "tipo": "medio"
},
{
    "codigo": 40,
    "nombre": "Handmade Frozen Salad",
    "unidades": 13,
    "precio": 85,
    "fabricante": "Nordstrom",
    "tipo": "medio"
},
{
    "codigo": 41,
    "nombre": "Awesome Cotton Cheese",
    "unidades": 56,
    "precio": 277,
    "fabricante": "HealthSouth",
    "tipo": "basico"
},
{
    "codigo": 42,
    "nombre": "Licensed Granite Ball",
    "unidades": 74,
    "precio": 92,
    "fabricante": "SunPower",
    "tipo": "medio"
},
{
    "codigo": 43,
    "nombre": "Sleek Frozen Table",
    "unidades": 50,
    "precio": 77,
    "fabricante": "Archrock",
    "tipo": "avanzado"
},
{
    "codigo": 44,
    "nombre": "Sleek Steel Ball",
    "unidades": 36,
    "precio": 236,
    "fabricante": "TransDigm Group",
    "tipo": "avanzado"
},
{
    "codigo": 45,
    "nombre": "Fantastic Soft Pants",
    "unidades": 78,
    "precio": 103,
    "fabricante": "TEGNA",
    "tipo": "basico"
},
{
    "codigo": 46,
    "nombre": "Intelligent Metal Bike",
    "unidades": 16,
    "precio": 141,
    "fabricante": "Core-Mark Holding",
    "tipo": "avanzado"
},
{
    "codigo": 47,
    "nombre": "Practical Frozen Chips",
    "unidades": 0,
    "precio": 305,
    "fabricante": "Delta Air Lines",
    "tipo": "medio"
},
{
    "codigo": 48,
    "nombre": "Refined Plastic Hat",
    "unidades": 52,
    "precio": 81,
    "fabricante": "Wendy's",
    "tipo": "basico"
},
{
    "codigo": 49,
    "nombre": "Licensed Concrete Soap",
    "unidades": 21,
    "precio": 68,
    "fabricante": "First Solar",
    "tipo": "basico"
},
{
    "codigo": 50,
    "nombre": "Awesome Frozen Shoes",
    "unidades": 33,
    "precio": 125,
    "fabricante": "Comerica",
    "tipo": "medio"
},
{
    "codigo": 51,
    "nombre": "Fantastic Metal Pants",
    "unidades": 5,
    "precio": 129,
    "fabricante": "OneMain Holdings",
    "tipo": "basico"
},
{
    "codigo": 52,
    "nombre": "Ergonomic Metal Hat",
    "unidades": 25,
    "precio": 85,
    "fabricante": "Kar Auction Services",
    "tipo": "basico"
},
{
    "codigo": 53,
    "nombre": "Licensed Plastic Hat",
    "unidades": 96,
    "precio": 38,
    "fabricante": "Best Buy",
    "tipo": "medio"
},
{
    "codigo": 54,
    "nombre": "Generic Metal Sausages",
    "unidades": 84,
    "precio": 77,
    "fabricante": "DST Systems",
    "tipo": "medio"
},
{
    "codigo": 55,
    "nombre": "Small Metal Tuna",
    "unidades": 46,
    "precio": 43,
    "fabricante": "Raymond James Financial",
    "tipo": "medio"
},
{
    "codigo": 56,
    "nombre": "Intelligent Frozen Sausages",
    "unidades": 3,
    "precio": 111,
    "fabricante": "A.O. Smith",
    "tipo": "basico"
},
{
    "codigo": 57,
    "nombre": "Practical Fresh Fish",
    "unidades": 69,
    "precio": 331,
    "fabricante": "Hartford Financial Services Group",
    "tipo": "avanzado"
},
{
    "codigo": 58,
    "nombre": "Refined Concrete Shirt",
    "unidades": 57,
    "precio": 49,
    "fabricante": "Simon Property Group",
    "tipo": "basico"
},
{
    "codigo": 59,
    "nombre": "Handcrafted Granite Chicken",
    "unidades": 26,
    "precio": 164,
    "fabricante": "Comcast",
    "tipo": "medio"
},
{
    "codigo": 60,
    "nombre": "Practical Frozen Salad",
    "unidades": 43,
    "precio": 250,
    "fabricante": "Nasdaq OMX Group",
    "tipo": "basico"
},
{
    "codigo": 61,
    "nombre": "Sleek Rubber Keyboard",
    "unidades": 82,
    "precio": 33,
    "fabricante": "Alere",
    "tipo": "basico"
},
{
    "codigo": 62,
    "nombre": "Ergonomic Steel Fish",
    "unidades": 10,
    "precio": 94,
    "fabricante": "HCA Holdings",
    "tipo": "avanzado"
},
{
    "codigo": 63,
    "nombre": "Rustic Plastic Mouse",
    "unidades": 5,
    "precio": 24,
    "fabricante": "Orbital ATK",
    "tipo": "avanzado"
},
{
    "codigo": 64,
    "nombre": "Awesome Cotton Mouse",
    "unidades": 39,
    "precio": 285,
    "fabricante": "Telephone & Data Systems",
    "tipo": "basico"
},
{
    "codigo": 65,
    "nombre": "Intelligent Soft Towels",
    "unidades": 19,
    "precio": 93,
    "fabricante": "Ascena Retail Group",
    "tipo": "avanzado"
},
{
    "codigo": 66,
    "nombre": "Incredible Concrete Fish",
    "unidades": 96,
    "precio": 336,
    "fabricante": "Darling Ingredients",
    "tipo": "medio"
}]);
```

3. Debes poner el resultado de las consultas en cada apartado

- Cuenta los productos de tipo “medio”, usando un método básico
```json
db.productos.find({ "tipo": "medio" }).count()
```

-- Resultado
```json
50
```

- Indicar con un distinct, las empresas (fabricantes) que hay en la colección
```json
db.productos.distinct("fabricante")
```
-- Resultado
```json
[
  'A.O. Smith',
  'Alere',
  'American Tire Distributors Holdings',
  'Anthem',
  'Archrock',
  'Ascena Retail Group',
  'AutoNation',
  'Best Buy',
  'CIT Group',
  'Cabot',
  'Comcast',
  'Comerica',
  'Core-Mark Holding',
  'DST Systems',
  'Darling Ingredients',
  'Delta Air Lines',
  'Delta Tucker Holdings',
  "Dick's Sporting Goods",
  'First Solar',
  'HCA Holdings',
  'Hanesbrands',
  'Hartford Financial Services Group',
  'Hawaiian Holdings',
  'HealthSouth',
  'Hyatt Hotels',
  'Kar Auction Services',
  'Kelly Services',
  'Kemper',
  'Kimberly-Clark',
  'Lennar',
  'Mercury General',
  'Mondelez International',
  'Motorola Solutions',
  'Nasdaq OMX Group',
  'National Oilwell Varco',
  'Nordstrom',
  'OneMain Holdings',
  'Oneok',
  'Orbital ATK',
  'Pep Boys-Mann',
  'Pool',
  'Precision Castparts',
  'Primoris Services',
  'Raymond James Financial',
  'Seaboard',
  'Securian Financial Group',
  'Simon Property Group',
  'State Farm Insurance Cos.',
  'State Street Corp.',
  'SunPower',
  'TEGNA',
  'Telephone & Data Systems',
  'Total System Services',
  'Tractor Supply',
  'TransDigm Group',
  'Trinity Industries',
  'TrueBlue',
  'Universal American',
  'Universal Health Services',
  'WGL Holdings',
  "Wendy's",
  'Werner Enterprises',
  'WestRock',
  'Williams-Sonoma'
]
```

- Usando aggregate, visualizar los productos que tengan más de 80 unidades
```json
db.productos.aggregate([{ $match: { "unidades": { $gt: 80 } } }])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce2'),
    codigo: 0,
    nombre: 'Fantastic Wooden Fish',
    unidades: 95,
    precio: 291,
    fabricante: 'Kimberly-Clark',
    tipo: 'avanzado'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce4'),
    codigo: 2,
    nombre: 'Small Soft Fish',
    unidades: 96,
    precio: 189,
    fabricante: 'Primoris Services',
    tipo: 'medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cee'),
    codigo: 12,
    nombre: 'Refined Concrete Salad',
    unidades: 90,
    precio: 129,
    fabricante: 'Universal Health Services',
    tipo: 'avanzado'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d00'),
    codigo: 30,
    nombre: 'Small Rubber Pants',
    unidades: 89,
    precio: 16,
    fabricante: 'Hanesbrands',
    tipo: 'basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d03'),
    codigo: 33,
    nombre: 'Generic Concrete Hat',
    unidades: 82,
    precio: 70,
    fabricante: 'American Tire Distributors Holdings',
    tipo: 'basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d17'),
    codigo: 53,
    nombre: 'Licensed Plastic Hat',
    unidades: 96,
    precio: 38,
    fabricante: 'Best Buy',
    tipo: 'medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d18'),
    codigo: 54,
    nombre: 'Generic Metal Sausages',
    unidades: 84,
    precio: 77,
    fabricante: 'DST Systems',
    tipo: 'medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1f'),
    codigo: 61,
    nombre: 'Sleek Rubber Keyboard',
    unidades: 82,
    precio: 33,
    fabricante: 'Alere',
    tipo: 'basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d24'),
    codigo: 66,
    nombre: 'Incredible Concrete Fish',
    unidades: 96,
    precio: 336,
    fabricante: 'Darling Ingredients',
    tipo: 'medio'
  }
]
```

- Con $project visualizar solo el nombre, unidades y precio de los productos que tengan menos de 10 unidades
```json
db.productos.aggregate([
  { $match: { "unidades": { $lt: 10 } } },
  { $project: { "nombre": 1, "unidades": 1, "precio": 1 } }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    nombre: 'Ergonomic Metal Ball',
    unidades: 5,
    precio: 246
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    nombre: 'Handmade Plastic Hat',
    unidades: 7,
    precio: 253
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf6'),
    nombre: 'Ergonomic Metal Table',
    unidades: 0,
    precio: 94
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d11'),
    nombre: 'Practical Frozen Chips',
    unidades: 0,
    precio: 305
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d15'),
    nombre: 'Fantastic Metal Pants',
    unidades: 5,
    precio: 129
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1a'),
    nombre: 'Intelligent Frozen Sausages',
    unidades: 3,
    precio: 111
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d21'),
    nombre: 'Rustic Plastic Mouse',
    unidades: 5,
    precio: 24
  }
]
```

- Con $project ponemos el fabricante pero le cambiamos el nombre por “empresa”. Usamos el mismo comando anterior
```json
db.productos.aggregate([
  { $match: { "unidades": { $lt: 10 } } },
  { $project: { "nombre": 1, "unidades": 1, "precio": 1, "empresa": "$fabricante" } }
])
```
-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    nombre: 'Ergonomic Metal Ball',
    unidades: 5,
    precio: 246,
    empresa: 'Seaboard'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    nombre: 'Handmade Plastic Hat',
    unidades: 7,
    precio: 253,
    empresa: "Dick's Sporting Goods"
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf6'),
    nombre: 'Ergonomic Metal Table',
    unidades: 0,
    precio: 94,
    empresa: 'Kelly Services'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d11'),
    nombre: 'Practical Frozen Chips',
    unidades: 0,
    precio: 305,
    empresa: 'Delta Air Lines'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d15'),
    nombre: 'Fantastic Metal Pants',
    unidades: 5,
    precio: 129,
    empresa: 'OneMain Holdings'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1a'),
    nombre: 'Intelligent Frozen Sausages',
    unidades: 3,
    precio: 111,
    empresa: 'A.O. Smith'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d21'),
    nombre: 'Rustic Plastic Mouse',
    unidades: 5,
    precio: 24,
    empresa: 'Orbital ATK'
  }
]
```

- Añadir a la consulta anterior un campo calculado que se llame total y que multiplique precio por unidades.
```json
db.productos.aggregate([
  { $match: { "unidades": { $lt: 10 } } },
  { $project: { 
      "nombre": 1, 
      "unidades": 1, 
      "precio": 1, 
      "empresa": "$fabricante", 
      "total": { $multiply: ["$precio", "$unidades"] } 
    } 
  }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    nombre: 'Ergonomic Metal Ball',
    unidades: 5,
    precio: 246,
    empresa: 'Seaboard',
    total: 1230
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    nombre: 'Handmade Plastic Hat',
    unidades: 7,
    precio: 253,
    empresa: "Dick's Sporting Goods",
    total: 1771
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf6'),
    nombre: 'Ergonomic Metal Table',
    unidades: 0,
    precio: 94,
    empresa: 'Kelly Services',
    total: 0
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d11'),
    nombre: 'Practical Frozen Chips',
    unidades: 0,
    precio: 305,
    empresa: 'Delta Air Lines',
    total: 0
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d15'),
    nombre: 'Fantastic Metal Pants',
    unidades: 5,
    precio: 129,
    empresa: 'OneMain Holdings',
    total: 645
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1a'),
    nombre: 'Intelligent Frozen Sausages',
    unidades: 3,
    precio: 111,
    empresa: 'A.O. Smith',
    total: 333
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d21'),
    nombre: 'Rustic Plastic Mouse',
    unidades: 5,
    precio: 24,
    empresa: 'Orbital ATK',
    total: 120
  }
]
```

- Hacer que el nombre salga en mayúsculas con el operador $toUpper
```json
db.productos.aggregate([
  { $match: { "unidades": { $lt: 10 } } },
  { $project: { 
      "nombre": { $toUpper: "$nombre" }, 
      "unidades": 1, 
      "precio": 1, 
      "empresa": "$fabricante", 
      "total": { $multiply: ["$precio", "$unidades"] } 
    } 
  }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    unidades: 5,
    precio: 246,
    nombre: 'ERGONOMIC METAL BALL',
    empresa: 'Seaboard',
    total: 1230
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    unidades: 7,
    precio: 253,
    nombre: 'HANDMADE PLASTIC HAT',
    empresa: "Dick's Sporting Goods",
    total: 1771
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf6'),
    unidades: 0,
    precio: 94,
    nombre: 'ERGONOMIC METAL TABLE',
    empresa: 'Kelly Services',
    total: 0
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d11'),
    unidades: 0,
    precio: 305,
    nombre: 'PRACTICAL FROZEN CHIPS',
    empresa: 'Delta Air Lines',
    total: 0
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d15'),
    unidades: 5,
    precio: 129,
    nombre: 'FANTASTIC METAL PANTS',
    empresa: 'OneMain Holdings',
    total: 645
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1a'),
    unidades: 3,
    precio: 111,
    nombre: 'INTELLIGENT FROZEN SAUSAGES',
    empresa: 'A.O. Smith',
    total: 333
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d21'),
    unidades: 5,
    precio: 24,
    nombre: 'RUSTIC PLASTIC MOUSE',
    empresa: 'Orbital ATK',
    total: 120
  }
]
```

- Añadir un campo calculado que ponga el nombre del producto y el tipo concatenado con el operador $concat. Le llamamos al campo “completo”
```json
db.productos.aggregate([
  { $match: { "unidades": { $lt: 10 } } },
  { $project: { 
      "nombre": { $toUpper: "$nombre" }, 
      "unidades": 1, 
      "precio": 1, 
      "empresa": "$fabricante", 
      "total": { $multiply: ["$precio", "$unidades"] },
      "completo": { $concat: ["$nombre", " - ", "$tipo"] }
    } 
  }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    unidades: 5,
    precio: 246,
    nombre: 'ERGONOMIC METAL BALL',
    empresa: 'Seaboard',
    total: 1230,
    completo: 'Ergonomic Metal Ball - medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    unidades: 7,
    precio: 253,
    nombre: 'HANDMADE PLASTIC HAT',
    empresa: "Dick's Sporting Goods",
    total: 1771,
    completo: 'Handmade Plastic Hat - medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf6'),
    unidades: 0,
    precio: 94,
    nombre: 'ERGONOMIC METAL TABLE',
    empresa: 'Kelly Services',
    total: 0,
    completo: 'Ergonomic Metal Table - avanzado'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d11'),
    unidades: 0,
    precio: 305,
    nombre: 'PRACTICAL FROZEN CHIPS',
    empresa: 'Delta Air Lines',
    total: 0,
    completo: 'Practical Frozen Chips - medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d15'),
    unidades: 5,
    precio: 129,
    nombre: 'FANTASTIC METAL PANTS',
    empresa: 'OneMain Holdings',
    total: 645,
    completo: 'Fantastic Metal Pants - basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1a'),
    unidades: 3,
    precio: 111,
    nombre: 'INTELLIGENT FROZEN SAUSAGES',
    empresa: 'A.O. Smith',
    total: 333,
    completo: 'Intelligent Frozen Sausages - basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d21'),
    unidades: 5,
    precio: 24,
    nombre: 'RUSTIC PLASTIC MOUSE',
    empresa: 'Orbital ATK',
    total: 120,
    completo: 'Rustic Plastic Mouse - avanzado'
  }
]
```

- Ordena el resultado por el campo “total”
```json
db.productos.aggregate([
  { $match: { "unidades": { $lt: 10 } } },
  { $project: { 
      "nombre": { $toUpper: "$nombre" }, 
      "unidades": 1, 
      "precio": 1, 
      "empresa": "$fabricante", 
      "total": { $multiply: ["$precio", "$unidades"] },
      "completo": { $concat: ["$nombre", " - ", "$tipo"] }
    } 
  },
  { $sort: { "total": 1 } }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf6'),
    unidades: 0,
    precio: 94,
    nombre: 'ERGONOMIC METAL TABLE',
    empresa: 'Kelly Services',
    total: 0,
    completo: 'Ergonomic Metal Table - avanzado'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d11'),
    unidades: 0,
    precio: 305,
    nombre: 'PRACTICAL FROZEN CHIPS',
    empresa: 'Delta Air Lines',
    total: 0,
    completo: 'Practical Frozen Chips - medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d21'),
    unidades: 5,
    precio: 24,
    nombre: 'RUSTIC PLASTIC MOUSE',
    empresa: 'Orbital ATK',
    total: 120,
    completo: 'Rustic Plastic Mouse - avanzado'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d1a'),
    unidades: 3,
    precio: 111,
    nombre: 'INTELLIGENT FROZEN SAUSAGES',
    empresa: 'A.O. Smith',
    total: 333,
    completo: 'Intelligent Frozen Sausages - basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d15'),
    unidades: 5,
    precio: 129,
    nombre: 'FANTASTIC METAL PANTS',
    empresa: 'OneMain Holdings',
    total: 645,
    completo: 'Fantastic Metal Pants - basico'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    unidades: 5,
    precio: 246,
    nombre: 'ERGONOMIC METAL BALL',
    empresa: 'Seaboard',
    total: 1230,
    completo: 'Ergonomic Metal Ball - medio'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    unidades: 7,
    precio: 253,
    nombre: 'HANDMADE PLASTIC HAT',
    empresa: "Dick's Sporting Goods",
    total: 1771,
    completo: 'Handmade Plastic Hat - medio'
  }
]
```

- Haciendo una nueva consulta, averiguar el numero de productos por tipo de producto
```json
db.productos.aggregate([
  { $group: { _id: "$tipo", count: { $sum: 1 } } }
])
```

-- Resultado
```json
[
  { _id: 'avanzado', count: 18 },
  { _id: 'basico', count: 24 },
  { _id: 'medio', count: 25 }
]
```

- Añadir el valor mayor y el menor
```json
db.productos.aggregate([
  { $group: { 
      _id: "$tipo", 
      count: { $sum: 1 },
      maxPrecio: { $max: "$precio" },
      minPrecio: { $min: "$precio" }
    } 
  }
])
```

-- Resultado
```json
[
  { _id: 'medio', count: 25, maxPrecio: 337, minPrecio: 16 },
  { _id: 'avanzado', count: 18, maxPrecio: 331, minPrecio: 18 },
  { _id: 'basico', count: 24, maxPrecio: 285, minPrecio: 16 }
]
```

- Añade el total de unidades por cada tipo
```json
db.productos.aggregate([
  { $group: { 
      _id: "$tipo", 
      count: { $sum: 1 },
      maxPrecio: { $max: "$precio" },
      minPrecio: { $min: "$precio" },
      totalUnidades: { $sum: "$unidades" }
    } 
  }
])
```

-- Resultado
```json
[
  {
    _id: 'medio',
    count: 25,
    maxPrecio: 337,
    minPrecio: 16,
    totalUnidades: 1224
  },
  {
    _id: 'avanzado',
    count: 18,
    maxPrecio: 331,
    minPrecio: 18,
    totalUnidades: 773
  },
  {
    _id: 'basico',
    count: 24,
    maxPrecio: 285,
    minPrecio: 16,
    totalUnidades: 1067
  }
]
```

- Con el operador $set y el operador “$substr” visualiza todos los datos del producto "Small Metal Tuna" y los primeros 5 caracteres del nombre.
```json
db.productos.aggregate([
  { $match: { "nombre": "Small Metal Tuna" } },
  { $set: { "nombreCorto": { $substr: ["$nombre", 0, 5] } } }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0d19'),
    codigo: 55,
    nombre: 'Small Metal Tuna',
    unidades: 46,
    precio: 43,
    fabricante: 'Raymond James Financial',
    tipo: 'medio',
    nombreCorto: 'Small'
  }
]
```

- Creamos una salida que tenga el nombre del articulo y el total (precio por unidades) y lo guardamos en una colección denominada productos2
```json
db.productos.aggregate([
  { $project: { 
      "nombre": 1, 
      "total": { $multiply: ["$precio", "$unidades"] }
    } 
  },
  { $out: "productos2" }
])
```

-- Resultado
```json

```

- Comprobamos que se ha creado
```json
db.productos2.find()
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce2'),
    nombre: 'Fantastic Wooden Fish',
    total: 27645
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce3'),
    nombre: 'Rustic Concrete Pants',
    total: 18414
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce4'),
    nombre: 'Small Soft Fish',
    total: 18144
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce5'),
    nombre: 'Practical Soft Pants',
    total: 2747
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    nombre: 'Ergonomic Metal Ball',
    total: 1230
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce7'),
    nombre: 'Small Steel Gloves',
    total: 1665
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce8'),
    nombre: 'Ergonomic Wooden Shirt',
    total: 14994
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce9'),
    nombre: 'Handmade Steel Chair',
    total: 5392
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cea'),
    nombre: 'Handcrafted Soft Gloves',
    total: 4512
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ceb'),
    nombre: 'Fantastic Concrete Salad',
    total: 12985
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    nombre: 'Handmade Plastic Hat',
    total: 1771
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ced'),
    nombre: 'Refined Wooden Tuna',
    total: 8480
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cee'),
    nombre: 'Refined Concrete Salad',
    total: 11610
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cef'),
    nombre: 'Unbranded Soft Fish',
    total: 9434
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf0'),
    nombre: 'Small Concrete Fish',
    total: 5040
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf1'),
    nombre: 'Refined Concrete Bike',
    total: 2700
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf2'),
    nombre: 'Tasty Cotton Pants',
    total: 3536
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf3'),
    nombre: 'Incredible Granite Gloves',
    total: 20590
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf4'),
    nombre: 'Practical Metal Mouse',
    total: 6650
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf5'),
    nombre: 'Handcrafted Steel Chicken',
    total: 6215
  }
]
```

- Hacemos un find para comprobar el resultado
```json
db.productos2.find()
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce2'),
    nombre: 'Fantastic Wooden Fish',
    total: 27645
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce3'),
    nombre: 'Rustic Concrete Pants',
    total: 18414
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce4'),
    nombre: 'Small Soft Fish',
    total: 18144
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce5'),
    nombre: 'Practical Soft Pants',
    total: 2747
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    nombre: 'Ergonomic Metal Ball',
    total: 1230
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce7'),
    nombre: 'Small Steel Gloves',
    total: 1665
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce8'),
    nombre: 'Ergonomic Wooden Shirt',
    total: 14994
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce9'),
    nombre: 'Handmade Steel Chair',
    total: 5392
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cea'),
    nombre: 'Handcrafted Soft Gloves',
    total: 4512
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ceb'),
    nombre: 'Fantastic Concrete Salad',
    total: 12985
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    nombre: 'Handmade Plastic Hat',
    total: 1771
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ced'),
    nombre: 'Refined Wooden Tuna',
    total: 8480
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cee'),
    nombre: 'Refined Concrete Salad',
    total: 11610
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cef'),
    nombre: 'Unbranded Soft Fish',
    total: 9434
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf0'),
    nombre: 'Small Concrete Fish',
    total: 5040
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf1'),
    nombre: 'Refined Concrete Bike',
    total: 2700
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf2'),
    nombre: 'Tasty Cotton Pants',
    total: 3536
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf3'),
    nombre: 'Incredible Granite Gloves',
    total: 20590
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf4'),
    nombre: 'Practical Metal Mouse',
    total: 6650
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf5'),
    nombre: 'Handcrafted Steel Chicken',
    total: 6215
  }
]
```

- Usando $cond y $project vamos a visualizar el nombre del producto, el precio y un campo llamado valoración que ponga “barato” si el precio es menor de 250 y caro si es mayor o igual
```json
db.productos.aggregate([
  { $project: { 
      "nombre": 1, 
      "precio": 1, 
      "valoracion": { 
        $cond: { if: { $lt: ["$precio", 250] }, then: "barato", else: "caro" } 
      }
    } 
  }
])
```

-- Resultado
```json
[
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce2'),
    nombre: 'Fantastic Wooden Fish',
    precio: 291,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce3'),
    nombre: 'Rustic Concrete Pants',
    precio: 279,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce4'),
    nombre: 'Small Soft Fish',
    precio: 189,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce5'),
    nombre: 'Practical Soft Pants',
    precio: 67,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce6'),
    nombre: 'Ergonomic Metal Ball',
    precio: 246,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce7'),
    nombre: 'Small Steel Gloves',
    precio: 37,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce8'),
    nombre: 'Ergonomic Wooden Shirt',
    precio: 238,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ce9'),
    nombre: 'Handmade Steel Chair',
    precio: 337,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cea'),
    nombre: 'Handcrafted Soft Gloves',
    precio: 282,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ceb'),
    nombre: 'Fantastic Concrete Salad',
    precio: 265,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cec'),
    nombre: 'Handmade Plastic Hat',
    precio: 253,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0ced'),
    nombre: 'Refined Wooden Tuna',
    precio: 212,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cee'),
    nombre: 'Refined Concrete Salad',
    precio: 129,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cef'),
    nombre: 'Unbranded Soft Fish',
    precio: 178,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf0'),
    nombre: 'Small Concrete Fish',
    precio: 126,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf1'),
    nombre: 'Refined Concrete Bike',
    precio: 180,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf2'),
    nombre: 'Tasty Cotton Pants',
    precio: 52,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf3'),
    nombre: 'Incredible Granite Gloves',
    precio: 290,
    valoracion: 'caro'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf4'),
    nombre: 'Practical Metal Mouse',
    precio: 190,
    valoracion: 'barato'
  },
  {
    _id: ObjectId('67da27c8b8669e50b9cb0cf5'),
    nombre: 'Handcrafted Steel Chicken',
    precio: 113,
    valoracion: 'barato'
  }
]
```