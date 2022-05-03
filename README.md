# metodos-arrays-js

## MAP

### ejercicio 1

Crear una función que reciba un array de nombre de ciudades y devuelva un array con la primera letra de cada ciudad en mayúsculas. Ejemplo:

```js
["miami","barcelona","tokio"] ===> ["Miami", "Barcelona", "Tokio"]
```

Pasos:
- Crea una función `capitalize()` que realice las siguientes tareas:
   1. Obtenga el primer carácter de una cadena
   2. Convierta en mayúsculas el primer carácter de una cadena
   3. Concatene el carácter en mayúsculas al resto de la cadena (sin el primer carácter)

- Crea una función `capitalizeArray` que utilice la función anterior para modificar todos los elementos de un array. Obligatorio utilizar la función **array.map**


### ejercicio 2

Imaginad que sois profesores y queréis calificar a los estudiantes en función de sus resultados en 2 proyectos (40% de la nota final) y el examen final (60% de la nota final). La información de partida es la siguiente:

```javascript
        let  students = [
        {
          name: "Tony Parker",
          firstProject: 80,
          secondProject: 75,
          finalExam: 90
        },
        {
          name: "Marc Barchini",
          firstProject: 84,
          secondProject: 65,
          finalExam: 65
        },
        {
          name: "Claudia Lopez",
          firstProject: 45,
          secondProject: 95,
          finalExam: 99
        },
        {
          name: "Alvaro Briattore",
          firstProject: 82,
          secondProject: 92,
          finalExam: 70
        },
        {
          name: "Isabel Ortega",
          firstProject: 90,
          secondProject: 32,
          finalExam: 85
        },
        {
          name: "Francisco Martinez",
          firstProject: 90,
          secondProject: 55,
          finalExam: 78
        },
        {
          name: "Jorge Carrillo",
          firstProject: 83,
          secondProject: 77,
          finalExam: 90
        },
        {
          name: "Miguel López",
          firstProject: 80,
          secondProject: 75,
          finalExam: 75
        },
        {
          name: "Carolina Perez",
          firstProject: 85,
          secondProject: 72,
          finalExam: 67
        },
        {
          name: "Ruben Pardo",
          firstProject: 89,
          secondProject: 72,
          finalExam: 65
        }
        ]
   ```
Cread una función `calcFinalGrade()` que reciba un objeto como el anterior, como parámetro, y devuelva un array de objetos con los campos `name` y `final_grade`.



## REDUCE

### ejercicio 3

Crea una función `calcAverageCalories()` que reciba un objeto como el que se proporciona y devuelva la **media** de calorías de todo el menú. Utiliza la función reduce para calcularlo.

Los datos de partida deben tener la siguiente estructura:

```
let menu = [
  { name: "Carrots", calories: 150 },
  { name: "Steak", calories: 350 },
  { name: "Broccoli", calories: 120 },
  { name: "Chicken", calories: 250 },
  { name: "Pizza", calories: 520 }
];
```

### ejercicio 4


![Imgur](https://i.imgur.com/W7R22Cw.png)

Estamos desarrollando nuestro super e-commerce, cada producto tiene comentarios de usuario y una puntuación almacenada en un array con el nombre de `reviews`. Cada `review` tiene la siguiente estructura:

```javascript
let product = {
  name: "JIM'S STORE 2 Bobina 10W Cargador Inalámbrico Titular Anti-Deslizamiento Diseño",
  price: 15.69,
  manufacturer: "JIM'S STORE",
  reviews:
  [
    {  user: "Pavel Nedved",
      comments: "Muy contento",
      rate: 4
    },
    {  user: "Alvaro Trezeguet",
      comments: "No tiene carga rápida",
      rate: 1
    },
    {  user: "David Recoba",
      comments: "Excelente relación calidad/precio.",
      rate: 5
    },
    {  user: "Maribel Romero",
      comments: "Pocas prestaciones",
      rate: 2
    },
    {  user: "Antonio Cano",
      comments: "Materiales malos",
      rate: 1
    },
  ]
}

```
Queremos mostrar el producto en nuestra web pero no queremos mostrar todos los comentarios de primera vista. Sólo necesitamos la valoración media para que los clientes se hagan una idea rápida de la valoración del producto.

Crea una función que calcule la media de las valoraciones de los clientes y el test que pruebe la función (_tip_: misma estructura que el test de la función anterior)

### BONUS
Traslada la media a pintar "estrellas" de valoración en una página web con la imagen del producto.
