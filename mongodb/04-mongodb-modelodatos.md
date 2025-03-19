# Modelo de datos en mongodb

- Modelos
    - Embebidos
    - Referenciados
    
## Modelos Embebidos
**Uno a uno**
```json
db.departamentos.insertMany([
    {
        _id:1,
        nombre:"Tecnologias de informacion",
        responsable:{
            nombre:"Monico",
            apellidos:"Martinez Perez",
        },
        descripcion:"Ejemplo de departamento"
    },
    {
        _id:2,
        nombre:"Contabilidad",
        responsable:{
            nombre:"Raul",
            apellidos:"Lopez Hernandez",
        },
        descripcion:"Ejemplo de departamento"
    }    
])
```

- Modelos Referenciados
**Uno a Uno**
```json
db.localidades.insertMany(
{
    _id:'BA',
    ciudad: 'Buenos Aires',
    pais: 'Argentina',
    poblacion: '16 millones',
    turismo: ["edificios","tango","gastronomia","museos","parques"],
    direccion:"Avenida Tortolos",
    cod_departamento:1
},
{
    _id:'BA',
    ciudad: 'Santiago',
    pais: 'Chile',
    poblacion: '20 millones',
    turismo: ["iglesias","vino","gastronomia","museos","parques"],
    direccion:"Calle soy la vaca del corral",
    cod_departamento:2
})
```
```json
db.departamentos.aggreagate(
    [
        {
            $lookup:{
                from:"localidades",
                localField:"_id"
                foreingField:"cod_departamento"
                as "localidades"
            }
        }
    ]
)
```