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

