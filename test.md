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

    var completename = name + " " + lastname;

    return console.log("Mi nombre es " + completename + ",Pero prefiero que me digas " + nickname);

}

nombre(name,lastname,nickname);
