# Hello-World
Repositorio Universidad Java
CICLOS

  CICLO WHILE
       //definimos una variable (contador)
       //incrementamos la variable cierta cantidad de veces (3 veces)
       //agregamos la condicion (si el contador es <3 entonces se seguira ejecutando esta condicion)
       //y si la condicion que estamos proporcionando es verdadera, se seguira ejecutando el bloque de codigo dentro de la esctructura while
       var contador = 0;
       while (contador < 3) {
           System.out.println("contador = " + contador);
           contador++;
       }
  CICLO DO WHILE

	var contador = 0;
         do {
             System.out.println("contador = " + contador);
             contador++;
         }while (contador > 3); 
 
   CICLO FOR
	
	//las sentencias que se van a repetir hasta que la condicion sea falsa
	//la primera parte del ciclo for la vamos a utilizar para declara nuestra variable de "contador la cual despues se va a incrementar posteriorme, de que termine de ejecutar las sentencias
	//la segunda parte es la condicion, y si es verdadera se ejecutan las lineas de codigo que estaran en la parte de abajo dentro del ciclo
	//finalmente la utima parte es para incrementar la parte de la variable "contador" que se ha definido al inicio, y esta parte se va a ejecutar una vez que haya terminado de evaluar las lineas de codigo cuando se realiza la repeticion, se revisa el incremento de la variable de contador, y se vuelve a revisar la condicion.
	//y de nueva cuenta si la condicion es verdadera se vuelven a ejecutar las lineas de codigo, se vueleve a revisar el incremento del contador y se vuelve a revisar la condicion, ese es el ciclo.

	 for( var contador = 0 ; contador < 3 ; contador++ ){
             System.out.println("contador = " + contador); 
        }

 EJEMPLO IF-ELSE / SWITCH
	int tasaEstandar = 90;
        char categoriaProfesional;
        
        if (tasaEstandar < 80){
            categoriaProfesional = 'C';
        }else
        if (tasaEstandar < 120){
                categoriaProfesional = 'B';
        }else{
            categoriaProfesional = 'A';
        }
           
        System.out.println("Tasa " + tasaEstandar + " euros "); 
        System.out.println("categoria " + categoriaProfesional + " de ");       
     
        switch (categoriaProfesional) {
            case 'A': System.out.println("Socio");
            break;
            case 'B': System.out.println("senior");
            break;
            case 'C': System.out.println("junior");
            break;
            default: System.out.println("Indefinida");
            break;
        }

 BREAK 
	//La palabra break nos va a permitir romper un ciclo, en este caso el ciclo "for"
	//en el ejmplo imprimiremos solamnete los numero pares que son multiplos de 2 (0 y 2) (exceptuando el valor de 1)
	//para esto ocuparemos el metodo "if" para preguntar si la variable que contiene nuestro numero  en este caso de "contador" aplicando el operador de modulo es igual a cero (numero par)
	//pero si quisieramos imprimir solamente el primer numero par que hemos encontrado (0 y 2), para ello usamos la palabra reservada break, para romper el ciclo, una vez que hallamos encontrado el numero buscado (el primer numero para de los elementos que estamos buscando)
	//si quitamos el break se imprimen todos los numeros pares
	
	for (int contador = 0; contador < 3; contador++) {
            if (contador % 2 == 0) {
                System.out.println("contador = " + contador);
                break;
            }
        }

 CONTINUE
	//en este caso invertiremos la logica, preguntando si el numero NO es un numero par	 
	//sacamos la linea de impresion y usamos la palabra continue
 	//continue ira a la siguiente iteracion del ciclo "for"
	//por lo tanto si la iteracion es verdadera, (no es numero par), nos vamos a la siguiente iteracion y ya no imprime el contador
	//en cambio si la expresion es falsa, esto quiere decir que es un "numero par"

	 for (int contador = 0; contador < 3; contador++) {
            if (contador % 2 != 0) {
                continue;
            }
            System.out.println("contador = " + contador);
        }

 CLASES 
	 package clases;
public class Persona {
  	//atributos de la clase
    	String nombre;
    	String apellido;
    
    	public void desplegarInformacion(){
        System.out.println("Nombre: " + nombre);
        System.out.println("Apellido: " + apellido);
 
PRUEBA CLASE

	package clases;
public class PruebaPersona {
    public static void main(String[] args) {
        Persona persona1 = new Persona();
        persona1.nombre = "Juan";
        persona1.apellido = "Perez";
        persona1.desplegarInformacion();
        
        Persona persona2 = new Persona();
        System.out.println("persona1 = " + persona1);
        System.out.println("persona2 = " + persona2);
        
        persona2.desplegarInformacion();
        persona2.nombre = "Karla";
        persona2.apellido = "Lara";
        persona2.desplegarInformacion();

CLASE ARITMETICA

	package Operaciones;
public class Aritmetica {
    	//atributos de la clase
    	int a;
    	int b;
    	
	//metodo
    	public void sumar(){
        int resultado = a + b;
        }
	public int sumarConRetorno() {
        return a + b;
    	}
      public int sumarConArgumentos(int arg1, int arg2){
      a = arg1;
      b = arg2;
      return sumarConRetorno();
    }
  }
 
PRUEBA ARITMETICA
	package Operaciones;


public class PruebaAritmetica {
    public static void main(String[] args) {
        Aritmetica aritmetica1 = new Aritmetica();
        aritmetica1.a = 3;
        aritmetica1.b = 2;
        aritmetica1.sumar();
        
        int resultado = aritmetica1.sumarConRetorno();
        System.out.println("resultado = " + resultado);
		
	resultado = aritmetica1.sumarConArgumentos(5, 8);
        System.out.println("resultado usando argumentos: = " + resultado);
       	}
  }

  THIS (CLASE ARITMETICA) Y CONSTRUCTOR

public class Aritmetica {
    //atributos
    int a;
    int b;
	
    //constructor vacio
    public Aritmetica(){
        System.out.println("Ejecutando constructor");

    //metodo
    public void sumar() {
        int resultado = this.a + this.b;
    }

    public int sumarConRetorno() {
        return this.a + this.b;
    }
    public int sumarConArgumentos(int a, int b){
         this.a = a;//el argumento a se asigna al atributo thin.a
         this.b = b;
        return this.sumarConRetorno();
    }

SOBRECARGA DE CONSTRUCTORES
	//constructor vacio
    public Aritmetica(){
        System.out.println("Ejecutando constructor");
    }
    //constructor con argumentos
    public Aritmetica(int a, int b){
        this.a = a;
        this.b = b;
 
(METODO MAIN)SOBRE CARGA DE CONSTRUCTORES

	Aritmetica aritmetica1 = new Aritmetica();
        System.out.println("aritmetica1 a: " + aritmetica1.a); //0
        System.out.println("aritmetica1 b: " + aritmetica1.b); //0
        
        Aritmetica aritmetica2 = new Aritmetica(5 , 8);
        System.out.println("aritmetica2 a: " + aritmetica2.a); //5
        System.out.println("aritmetica2 b: " + aritmetica2.b); //8
 
 EJERCICIO CAJA (Caja.java)
	 
	package Operaciones;

public class Caja {
    int alto ;
    int ancho;
    int profundo;
    
    public Caja(){
        
    }
    public Caja(int a, int b, int c){
        this.alto = a;
        this.ancho = b;
        this.profundo = c;
    }
    public void calcularVolumen(){
        int resultado = this.alto * this.ancho * this.profundo;
        System.out.println("resultado = " + resultado);
    }
    
    public int calcularVolumenCon(int a, int b, int c){
        this.alto = a;
        this.ancho = b;
        this.profundo = c;
        return this.alto * this.ancho * this.profundo; 
    } 
	EJERCICIO CAJA (PruebaCaja.java)
	 
	package Operaciones;


public class PruebaCaja {
    public static void main(String[] args) {
        Caja volumenCaja = new Caja();
        volumenCaja.alto = 3;
        volumenCaja.ancho = 2;
        volumenCaja.profundo = 6;
        volumenCaja.calcularVolumen();
