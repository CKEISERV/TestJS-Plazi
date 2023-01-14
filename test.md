## Variables y Operaciones

## 1. Responde las siguientes preguntas

a. Que es una variable y para que sirve? -> Una variable es un espacio en memoria que permite almacenar datos o información

b. Cual es la diferencia entre declarar e inicializar una variable? -> Declarar es crear y determinar el tipo de variable con su nombre (let nombre). Inicializar es otorgarle un valor a la variable declarada (nombre = "Cesar")

c. Cual es la diferencia entre sumar y concatenar strings. Cual operador permite esto -> El operador utilizado es "+". Al sumar dos numeros el resultado esperado es el valor de la suma(2 + 2 = 4), mientras que al concatenar strings nos regresa ambos valores unidos("2" + "2" = 22).

## 2. Determina el nombre y el tipo de dato para almacenar en variables la siguiente información

a. Nombre -> String
b. Apellido -> String
c. Nombre de usuario en Platzi -> String
d. Edad -> Numero
e. Correo electronico -> String
f. Mayor de edad -> booleano
h. Dinero ahorrado -> numero
i. Deudas -> numero

## 3. Traduce a codigo JavaScript las variables del ejemplo anterior

let nombre = "Cesar";
let apellido = "Villamizar";
let userName = "CKEISERV";
let edad = 24;
let email = "cesar.villamizar@gmail.com"
let esMayorDeEdad = true;
let dineroAhorrado = 150000;
let deudas = 50000;

## 4. Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

a. Nommbre completo ->
let completeName = nombre + " " + apellido;

b. Dinero Real ->
let dineroReal = dineroAhorrado - deudas;

## Funciones

## 1. Responde las siguientes preguntas

a. Que es una función -> Una función es un conjunto de acciones que nos devuelve un resultado. Nos permite guardar bloques de codigo para reutilizarlos y ejecutarlos en el futuro

b. Cuando me sirve usar una función en mi codigo? -> Cuando tenemos codigo repetido. Igualmente cuando el codigo es bastante extenso, se encapsula parte del codigo que tenga relación para una mejor comprensión del codigo

c. Cual es la diferencia entre parametros y argumentos de una función? -> Los parametros son los recibidos por la función cuando son declaradas. Los argumentos son los enviados cuando las funciones son ejecutadas

## 2. Convierte el siguiente codigo en una función, pero cambiando cuando sea necesario las variables constantes por parametros y argumentos en una funcion

a.

const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");

-->

let name = "cesar";
let lastname = "villamizar";
let nickname = "ckeiserv";

function nombre(name,lastname,nickname){

    let completename = name + " " + lastname;

    return console.log("Mi nombre es " + completename + ",Pero prefiero que me digas " + nickname);

}

nombre(name,lastname,nickname);

## Condicionales

## 1. Responde las siguientes preguntas

a. Que es un condicional -> Es un codigo que compara una condición o validación y dependiendo de ello, ejecuta una acción u otra

b. Que tipos de condicionales existen en JS y sus diferencias -> IF (else, else if) y Switch. En el caso de switch siempre se evalua la misma validación de la variable, caso contrario del if que permite realizar validaciones distintas si así queremos

c. Puedo combinar funciones y condicionales? -> Si se puede.

## 2. Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

a. const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
case "Free":
console.log("Solo puedes tomar los cursos gratis");
break;
case "Basic":
console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
break;
case "Expert":
console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
break;
case "ExpertPlus":
console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
break;
}

-->

const tipoDeSuscripcion = "Basic";

if(tipoDeSuscripción === "Free"){
console.log("Solo puedes tomar los cursos gratis");

}else if(tipoDeSuscripción === "Basic"){
console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");

}else if(tipoDeSuscripción === "Expert"){
console.log("Puedes tomar casi todos los cursos de Platzi durante un año");

}else if(tipoDeSuscripción === "ExpertPlus"){
console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

## Ciclos

## 1. Responde las siguientes preguntas

a. Que es un ciclo? -> Es un bloque de codigo que ejecuta una determinada acción hasta que se cumpla la condición dada

b. Que te tipos de ciclos existen en JavaScript? -> for, while y do while

c. Que es un ciclo infinito y porque es un problema? -> Un ciclo infinito es cuando no hay una acción que interrumpa su ejecución, con ello el resto del codigo no va a compilar y se termina dañando la ejecución

d. Puedo mezclar ciclos y condicionales? Si se puede

## 2. Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

a. for (let i = 0; i < 5; i++) {
console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
console.log("El valor de i es: " + i);
}

-->

let i = 0;

while(i < 5){
console.log("El valor de i es " + i);
i++;
}

let i = 10

while(i>=2){
console.log("El valor de i es: " + i);
i--;
}

## 3. Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar

let resultado = 4;

let pregunta = prompt("Cuanto es el resultado de 2 + 2");

let respuesta = parseInt(pregunta);

while(resultado != respuesta){

console.log("volvamos a empezar");

pregunta = prompt("Cuanto es el resultado de 2 + 2");

respuesta = parseInt(pregunta);

}

console.log("Felicitaciones");

## Listas

## 1. Responde las siguientes preguntas

a. Que es un array --> Es una lista de elementos

b. Que es un objeto --> Es una lista de elementos pero cada elemento tiene un nombre clave

c. Cuando es mejor usar objetos o arrays --> Arrays cuando lo que haremos en un elemento es lo mismo que en todos los demas. Mientras que en un objeto cuando los nombres de cada elemento son importantes para nuestro algoritmo

d. Puedo mezclar arrays con objetos o incluso objetos con arrays? --> si se puede

## 2. Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

let primerElemento = [0,1,2,3,4,5]

function imprimir(primerElemento){

    console.log(primerElemento[0]);

}

imprimir(primerElementor);

## 3. Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

let todosLosElementos = [1,2,3];

function imprimirTodos(elementos){

    for(let i = 0; i< elementos.length; i++){
        console.log(elementos[i])
    }

}

imprimirTodos(todosLosElementos);

## 4. Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

let todoslosElementos = {

    nombre: "Cesar",
    apellido: "Villamizar",
    edad: 24

}

function imprimirTodos(elementos){
let elementosArray = Object.values(elementos);

        for(let i = 0; i< elementosArray.length; i++){
        console.log(elementosArray[i])
    }

}

imprimirTodos(todoslosElementos)

## Bonus

## Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
case "Free":
console.log("Solo puedes tomar los cursos gratis");
break;
case "Basic":
console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
break;
case "Expert":
console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
break;
case "ExpertPlus":
console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
break;
}

-->

function tipoDeSuscripción(subscripción){
if(subscripción === "Free"){
console.log("Solo puedes tomar los cursos gratis");
return;
}

if(subscripción === "Basic"){
console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
return;
}

if(subscripción === "Expert"){
console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
return;
}

if(subscripción === "ExpertPlus"){
console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
return;
}

console.log("No existe el tipo de subscripción")
}

## Replicar este comportamiento con arrays u objetos y un solo condicional.

const userSucription = "Basic";

let typeSuscription = [
"Free",
"Basic",
"Expert",
"ExpertPlus" ];

let infoSuscription = [
"solo puedes tomar los cursos gratis",
"puedes tomar casi todos los cursos de Platzi durante un mes",
"puedes tomar casi todos los cursos de Platzi durante un año",
"tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"];

    for(let i = 0; i<=typeSuscription.length; i++){
        if(userSucription === typeSuscription[i]){
            console.log(`Su susbcripcion es ${typeSuscription[i]} por lo tanto ${infoSuscription[i]}`)
        }
    }
