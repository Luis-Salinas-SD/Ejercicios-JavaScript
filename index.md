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
