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
