## Ejercicios de JavaScript

1. Programa una función que cuente el número de caracteres de una cadena de texto.

- ("Hola Mundo") devolverá 10.

```javascript
let txt = "Hola Mundo";
function count(txt) {
  a = txt.length;
  console.log(a);
}
count(txt);
```

2. Programa una función que te devuelva el texto recortado según el número de caracteres indicados.

- miFuncion("Hola Mundo", 4) devolverá "Hola".

```javascript
let txt = "Hola Mundo";
function r(txt) {
  console.log(txt.slice(0, 4));
}
r(txt);
```

3. Programa una función que dada una String te devuelva un Array de textos separados por cierto caracter.

- miFuncion('hola que tal', ' ') devolverá ['hola', 'que', 'tal'].

```javascript
let txt = "Hola que tal";
function r(txt) {
  console.log(txt.split(" "));
}
r(txt);
```

4. Programa una función que repita un texto "N" veces.

- miFuncion('Hola Mundo', 3) devolverá Hola Mundo Hola Mundo Hola Mundo.

```javascript
let txt = "Hola que tal";
function r(txt) {
  for (let i = 1; i <= 5; i++) {
    console.log(i + " " + txt);
  }
}
r(txt);
```
5. programa una funcion que invierta el texto
- hola mundo 

```javascript
let txt = "Hola mundo";
function reversa(txt) {
  let arr = txt.split("").reverse().join("");

  console.log(arr);
}
reversa(txt);
```
6. Programa una función para encontrar el número de veces que se repite una palabra en un texto largo
- Hola mundo adíos mundo

```javascript
let texto = "hola mundo adios mundo mundo mundo";

let b = "mundo";
function resolv() {
  let i = 0; //indice //6 //18 //24 //30 //-1
  let count = 0; //contador //1 //2 //3 //4

  while (i !== -1) {
    i = texto.indexOf(b, i); //5 //17 //23 //29 //-1
    if (i !== -1) {
      //console.log(i);
      i++; //6 //18 //24 //30
      count++; //1 //2 //3 //4
    } //if
  } //while

  console.log(
    `La Palabra ${b} se encuentra ${count} veces en el texto anterior`
  );
}
resolv(texto, b);
```
7. Programa una función que te diga si una palabra o frase es un palindromo o no.
- "Hola mundo adíos mundo"
- 
```javascript
let word = prompt("Escribe la palabra");
function palindromo(word) {
  word = word.toLowerCase(); //el texto lo convierte a minisculas.
  let r = word.split("").reverse().join(""); //el texto lo convierte a arreglo, lo invierte y al final lo une
  console.log("La palabra original:" + word);

  console.log("Palabra al reves:" + r);
  if (word === r) {
    console.log("es palindromo");
  } else {
    console.log("no es");
  }
}
palindromo(word);
```

8. Programa una función que te diga si una palabra o frase es un palindromo o no.
- "Hola mundo adíos mundo"
