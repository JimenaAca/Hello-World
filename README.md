# Hello-World
Repositorio Universidad Java

import java.util.Scanner;
//Mi clase en Java
public class HolaMundo {
    public static void main (String args[]) {
int miVariableEntera = 10;
     System.out.println(miVariableEntera);
miVariableEntera = 5;
     System.out.println(miVariableEntera);
String miVariableCadena = "Saludos";
     System.out.println(miVariableCadena);
miVariableCadena = "Adios";
      System.out.println(miVariableCadena);

 VAR       
 
var miVariableVar = 20;
     System.out.println(miVariableVar);
miVariableVar = 50;
     System.out.println(miVariableVar);
var miVariableCadena = "Hola Mundo";
     System.out.println("miVariableCadena = " + miVariableCadena);
var titulo = "Ingeniero";
var usuario = "Juan";
var union = titulo + " " + usuario;
     System.out.println("union = " + union);
var i = 3;
var j = 4; 

//se realiza la suma de números
     System.out.println(i + j);   //7

//evaluacion de izquiera a derecha realiza suma
     System.out.println(i+ j + usuario);    //7Juan

//contexto cadena todo es una cadena
     System.out.println(usuario + i + j);    //Juan34
//uso de parentesis modifican la prioridad en la evaluación
     System.out.println(usuario + (i + j));    //Juan7

//salto de linea 
var nombre = "Karla";
     System.out.println("Nueva linea \n" + nombre);

//tabuelador
     System.out.println("Tabulador \t " + nombre);
//retroceso
     System.out.println("Retroceso \b " + nombre);
//comilla simple
     System.out.println("Comilla simple \'" + nombre + "\'");
//comilla doble 
     System.out.println("Comilla doble \"" + nombre + "\"");
        
SCANNER
      System.out.println("Escribe tu nombre;");
Scanner consola = new Scanner(System.in);
String nombre = consola.nextLine();
      System.out.println("Escribe tu profesion:");
String profesion = consola.nextLine();
     System.out.println(profesion + " " + nombre);
     System.out.println("proporciona el titulo");
Scanner consola = new Scanner(System.in);
String titulo = consola.nextLine();
      System.out.println("proporciona el nombre del autor:");
String autor = consola.nextLine();
      System.out.println(titulo + " " + "fue escrito por" + " " + autor);
         /* 
 tipos primitivos enteros: byte(8 bits), short(16), int(32), long(64)...
*/
byte numeroByte = (byte) 129;   //-128
      System.out.println("numeroByte = " + numeroByte);
      System.out.println("valor maximo" + Byte.MAX_VALUE);   //127
      System.out.println("valor minimo" + Byte.MIN_VALUE);   //-128
short numeroShort = (short) 32768;   //-32768
      System.out.println("numeroShort = " + numeroShort);
      System.out.println("valor maximo" + Short.MAX_VALUE);  //32767
      System.out.println("valor minimo" + Short.MIN_VALUE);  //-32768

int numeroInt = (int) 2147483648L;  //-2147483648
      System.out.println("numeroInt = " + numeroInt);
      System.out.println("valor maximo" + Integer.MAX_VALUE);   //2147483647
      System.out.println("valor minimo" + Integer.MIN_VALUE);   //-2147483648
long numeroLong = 9223372036854775807L; //9223372036854775807
      System.out.println("numeroLong = " + numeroLong);
      System.out.println("valor maximo" + Long.MAX_VALUE);   //9223372036854775807
      System.out.println("valor minimo" + Long.MIN_VALUE);   //-9223372036854775808

MI VARIABLE CHAR 

char miCaracter = 'a';
     System.out.println("miCaracter = " + miCaracter);
char varChar = '\u0021';
     System.out.println("varChar = " + varChar);
char miCaracterDecimal = 33;
     System.out.println("miCaracterDecimal = " + miCaracterDecimal);
char miCaracterSimbolo = '!';
     System.out.println("miCaracterSimbolo = " + miCaracterSimbolo);
        // codigo   signo   decimal
        //  u+0021     !        33
        //  u+0061     a        97
var varChar2 = '\u0021';
      System.out.println("varChar2 = " + varChar);   //!
var miCaracterDecimal2 = (char)33;
      System.out.println("miCaracterDecimal2 = " + miCaracterDecimal2);   //!
var miCaracterSimbolo2 = '!';
      System.out.println("miCaracterSimbolo2 = " + miCaracterSimbolo2);   //!
int miCaracterEntero = '!';
      System.out.println("miCaracterEntero = " + miCaracterEntero);   //33
BOOLEAN
boolean varBoolean = false;
 if (varBoolean){
      System.out.println("verdadero")
 }
 else {
     System.out.println("falso");
 }   
var edad = 10;
//var esMayorDeEdad = edad >= 18;
if (edad >= 18) {
      System.out.println("es mayor");
 }
else {
      System.out.println("es igual o menor");
  }

STRING A INT
var edad = Integer.parseInt("20");   //recordamos que al tener comillas dobles se convierte en cadena
     System.out.println("edad = " + edad);   //20(entero) 
var edad = “20”;  //20 concatenado con 1
     System.out.println("edad = " + edad + 1);    //201(vente-uno) string
// suma mas concatenacion  

System.out.println("edad = " + (edad + 1));   // 21(veintiuno)entero

PEDIR UN VALOR MEDIANTE EL METODO SCANNER
var edad = Integer.parseInt("20");
     System.out.println("edad = " + edad);

//pedir un valor

var consola = new Scanner(System.in);
     System.out.println("escribe tu edad: ");
edad = Integer.parseInt( consola.nextLine());
     System.out.println("edad = " + edad);

INT A STRING

var edadTexto = String.valueOf(10);
      System.out.println("edadTexto = " + edadTexto);    //”10” string

STRING A CHAR
var caracter = "hola".charAt(0);
     System.out.println("caracter = " + caracter);
      System.out.println("proporciona un caracter:");
var consola = new Scanner(System.in);
caracter = consola.nextLine().charAt(0);
     System.out.println("caracter = " + caracter);

EJERCIO 
import java.util.Scanner;
//Mi clase en Java
public class HolaMundo {
    public static void main (String args[]) {

 //Proporciona el nombre: (String)

 var nombre = "Programacion con Java";
      System.out.println("Proporciona el nombre: ");
Scanner consola = new Scanner(System.in);
nombre = consola.nextLine();
       
//Proporciona el id: (Int)

var id = Integer.parseInt("1520"); 
      System.out.println("Proporciona el id: ");
consola = new Scanner(System.in);
id = Integer.parseInt( consola.nextLine());
//Proporciona el precio: (Double)

var precio = Double.parseDouble("899.0");
     System.out.println("Proporciona el precio: ");
consola = new Scanner(System.in);
precio = Double.parseDouble( consola.nextLine());

//Proporciona el envio: (boolean)
var envio = true;
      System.out.println("Proporciona si el envio tiene costo: ");
if (envio) {
      System.out.println("con costo de envio");
 }    else {
      System.out.println("sin costo de envio");
 }
       
 USO DE OPERADORES
int a=3, b=2;
var resultado = a + b;
     System.out.println("resultado de suma = " + resultado);
resultado = a - b;
     System.out.println("resultado de resta = " + resultado);
resultado = a * b;
     System.out.println("resultado de multiplicacion = " + resultado);
        
 Double resultado2 = 3.0/b;
      System.out.println("resultado2 = " + resultado2);
 //sobrantes de la division
resultado = a % b;
     System.out.println("resultado = " + resultado);
        /* si el residuo del resultado de la divion de a/b es igual a cero es par
si es igual a 1 es impar
*/
if ( b % b == 0); //igualdad
     System.out.println("es par");
else
     System.out.println("es impar");

EJEMPLO

Scanner consola = new Scanner(System.in);
     System.out.println("proporciona el alto");
int a = Integer.parseInt(consola.nextLine());
     System.out.println("proporciona el ancho");
int b = Integer.parseInt(consola.nextLine());
a = 10;
b = 20;
int perimetro = (a + b) * 2;
      System.out.println("perimetro = " + perimetro);
int area = a * b;
     System.out.println("area = " + area);

OPERADORES DE ASIGNACION
int a = 3, b = 2;
int c = a + 5 - b;
     System.out.println("c = " + c);  //resultado: = 6

OPERADOR DE COMPOSICION
a += 1;//a = a + 1
     System.out.println("a = " + a); //4
a += 3;// a = a + 3
     System.out.println("a = " + a);  //7
a -= 2; // a = a – 2
     System.out.println("a = " + a);  //5
     
 // *= , /= , %= multiplicacion, division y asignacion
 a *= 5; //a = a * 5
     System.out.println("a = " + a); //15
a /= 5;  //a = a / 5
      System.out.println("a = " + a); //3
 a %= 2; //a = a % 2 (divisible entre 2)
       System.out.println("a = " + a); //1

OPERADORES UNARIOS
//cambio de signo
        var a = 3;
        var b = -a;
        System.out.println("a = " + a); //3
        System.out.println("b = " + b); //-3
                     
        //operador de negacion, aplica para variables de tipo boolean
        //invertimos el valor de c usando el operador unario de negacion
      
        var c = true;
        var d = !c; //false
        System.out.println("c = " + c);
        System.out.println("d = " + d);
        
        //incremento 
        //1. preincremento (simbolo antes de la variable)
        var e = 3;
        var f = ++e; //primero se incrementa la variable y despues se usa su valor
        System.out.println("e = " + e); //4
        System.out.println("f = " + f);  //4
        
        //2.posincremento (simbolo despues de la variable)
        var g = 5;
        var h = g++; //primero se utiliza el valor de la variable y luego se incrementa
        System.out.println("g = " + g); //6 (teniamos pendiente un incremento)
        System.out.println("h = " + h); //5
        
        //decremento
        //1.predecremento
        var i = 2;  
        var j = --i; 
        System.out.println("i = " + i); //1 (ya esta decrementada)
        System.out.println("j = " + j);  //1
        
        //2.posdecremento
        var k = 4;
        var l = k--;//primero se usa el valor de l avariable y queda pendiente l decremento
        System.out.println("k = " + k); //3 (queda pendiente un decremento)
        System.out.println("l = " + l); //4

OPERADORES DE IGUALDAD
var a = 3;
        var b = 2;
        
        //operador de igualdad, sirve para preguntar si dos elementos son iguales
        
       var c = a == b;
        System.out.println("c = " + c); //false
        
        //operador diferente de....
        var d = a != b;
        System.out.println("d = " + d); //true
        
        var cadena = "hola";
        var cadena2 = "adios";
        
        var e = cadena == cadena2; //compara referencias de objetos 
        System.out.println("e = " + e); //false
        
        //comparar el contenido de las cadenas, mediante el metodo .equals
        var f = cadena.equals(cadena2);
        System.out.println("f = " + f); //false
        

OPERADOPRES RELACIONLES
 //mayor...
        //var g = a > b;
        //System.out.println("g = " + g); //true
        //mayor o igual...
        var g = a >= b;
        System.out.println("g = " + g); //true

        var h = a < b;
        System.out.println("h = " + h); //false

        //par o inpar
        //si el residuo de dividir a(3) / b(2) es igual a 0 el resultado es par
        //si el residuo de dividir a / b es igual a 1 el resultado es impar
        if (a % 2 == 0) {
            System.out.println("es numero par: ");
        } else {
            System.out.println("es numero impar: "); //false
        }
        
        var edad = 30;
        var adulto = 18;
        
        if (edad >= adulto){
            System.out.println("es un adulto"); //true
        } else {
            System.out.println("es menor de edad");
        }       
        OPERADORES CONDICIONALES

//vamos a comprobar si esta variable se encuentra dentro de un rango, definimos un valor mínimo y un valor máximo… (0-10)
//el operador de “&&” solamente va a regresar “true” cuando ambas expresiones den “true”, si alguna de ellas da falso, entonces va a regresar “true”.
        var a = 0;
        var valorMinimo = 0;
        var valorMaximo = 10;

        //s1 a es mayor o igual que 0, cumple con el rango minimo
        //si a es menor o igual que 10, cumple con el valor maximo
        var resultado = a >= 0 && a <= 10;
        System.out.println("resultado = " + resultado); //true
        if (resultado) {
            System.out.println("dentro de rango");
        } else {
            System.out.println("fuera de rango");

PROCEDENCA DE OPERADORES EN JAVA
        var x = 5;
        var y = 10;
        var z = ++x + y--;
        System.out.println("x = " + x); //6    
        System.out.println("y = " + y); //9
        System.out.println("z = " + z); //16
        
        var x = 10;
        var y = 20;
        var z = ++x + y--;
        System.out.println("x = " + x); //11      
        System.out.println("y = " + y); //19
        System.out.println("z = " + z); //31
        
        var resultado = 4 + 5 * 6 / 3; //4 ((5 * 6)/3)= 14
        System.out.println("resultado = " + resultado);
        resultado = (4 + 5) * 6 / 3; //= 18
        System.out.println("resultado = " + resultado);
SENTENCIA DE CONTROL (IF)
	var condicion = true;
        if (condicion) {
            System.out.println("es verdadero");
            System.out.println("nueva linea");
        } else {
        }   System.out.println("es falso");

EJEMPLO
        int numero = 1;
        var numeroTexto = "numero desconocido";
        
        if (numero == 1) {
            System.out.println("numero uno");
        }
        else if (numero == 2) {
            System.out.println("numero dos");
        }
        else if (numero == 3) {
            System.out.println("numero tres");
        }
        else if (numero == 4) {
            
        }
        else {
            System.out.println("numero no encontrado");
        }

EJEMPLO 2 
	var mes = 13;
        var estacion = "Estacion desconocida";
        if (mes == 1 || mes == 2 || mes == 12) {
            estacion = "invierno";
        }
        else if (mes == 3 || mes == 4 || mes == 5) {
            estacion = "primavera";
        }
        else if (mes == 6 || mes == 7 || mes == 8) {
            estacion = "verano";
        }
        else if (mes == 9 || mes == 10 || mes == 11) {
            estacion = "otono";
        }
        System.out.println("estacion = " + estacion);

EJEMPLO 3 
	var consola = new Scanner(System.in);
        System.out.println("Proporciona el numero de mes");
        var mes = Integer.parseInt(consola.nextLine());
        var estacion = "Estacion desconocida";
        
        if (mes == 1 || mes == 2 || mes == 12) {
            estacion = "invierno";
        }
        else if (mes == 3 || mes == 4 || mes == 5) {
            estacion = "primavera";
        }
        else if (mes == 6 || mes == 7 || mes == 8) {
            estacion = "verano";
        }
        else if (mes == 9 || mes == 10 || mes == 11) {
            estacion = "otono";
        }
        System.out.println("estacion = " + estacion);

SENTENCIA DE CONTROL SWITCH EN JAVA 
	var numero = 2;
        var numeroTexto = "valor desconocido";

        switch (numero) {
            case 1:
                numeroTexto = "numero 1";
                break;
            case 2:
                numeroTexto = "numero 2";
                break;
            case 3:
                numeroTexto = "numero 3";
                break;
            case 4:
                numeroTexto = "numero 4";
                break;
            default: 
                numeroTexto = "caso no encontrado";
        }
        System.out.println("numeroTexto = " + numeroTexto);

EJEMPLO 
	Scanner consola = new Scanner(System.in);
        System.out.println("Proporciona el numero del mes que corresponda: ");
        var mes = Integer.parseInt(consola.nextLine());
        var estacion = "estacion desconocida";

        switch (mes) {
            case 1: case 2: case 12:
                estacion = "invierno";
                break;
            case 3: case 4: case 5:
                estacion = "primavera";
                break;
            case 6: case 7: case 8 :
                estacion = "verano";
                break;
            case 9: case 10: case 11:
                estacion = "otono";
                break;
        }
         System.out.println("estacion = " + estacion);      

Ejercicio 2 
	 Scanner consola = new Scanner(System.in);
        System.out.println("Proporciona un valor entre 0 y 10: "); 
        var valor = Integer.parseInt(consola.nextLine());
        var resultado = "valor desconocido";
        if (valor >= 9 && valor <= 10){
            System.out.println("A");
        }
        else if (valor >= 8 && valor < 9){
            System.out.println("B");
        }        
        else if (valor >= 7 && valor < 8){
            System.out.println("C");
        }        
        else if (valor >= 6 && valor < 7){
            System.out.println("D");
        }
        else if (valor >= 0 && valor < 6){
            System.out.println("F");
        }
        else{
            System.out.println("resultado = " + resultado);
        }
          

