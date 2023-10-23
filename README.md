# APOII

Curso de Algoritmos y Programacion II.

## Descripción
Registro de Actividades.

Se hizo un guardado rapido de los codigos realizados dentro la asignatura APOII 
a lo largo del segundo semestre de la Universidad Mariana con el objetivo de tener registro de ellos 
a modo de portafolio.

### Programas

Eclipse 
### ![ALT](https://2.bp.blogspot.com/-PqNShh8OyR0/WbnhQF1M_xI/AAAAAAAAM0Q/ZD4RsPm6hjkYrIGh61sTcY2HKxRJGsTuwCLcBGAs/s1600/eclipse-800x188.png)

### Instalación

1. Ingresa a la página oficial de Eclipse.

[anchor](https://www.eclipse.org/)

2. Presiona la opción "Download".

![Captura de pantalla_20230921_093554](https://github.com/JuanEraso23/APOII/assets/144852394/0d5d6a3a-3bdb-42e9-848a-b1c400e22f3a)

3. Presiona la opción "Download x86_64".

![Captura de pantalla_20230921_094130](https://github.com/JuanEraso23/APOII/assets/144852394/157499c8-1b34-4d20-868d-ff9f14355ba5)

4. Presiona la opción "Download".

![Captura de pantalla_20230921_094341](https://github.com/JuanEraso23/APOII/assets/144852394/19b85cd8-30c7-448e-8d4b-171914a3f9cb)

## Actividades

### Ejercicio 01
Calcula la distancia de un cuerpo según la velocidad y el tiempo.

_Sin Ingreso Por Teclado_

```
package ej01;

//Se reorganizo el codigo
public class SinIngresoPorTeclado {

	public static void main(String[] args) { 
		
		int d=0;
		int v=4;
		int t=8;
		      
		d=(v*t); 
		System.out.print("Distancia: "+d);    	  
	}	
}
```

_Scanner_

```
package ej01;

//Se reorganizo el codigo
//Se agrego "sc.close();"
import java.util.Scanner;

public class Ej01 {
	
      public static void main(String[] args) {
    	
            Scanner sc = new Scanner(System.in);
            
            System.out.print("Ingrese la Velocidad: ");
            int v = sc.nextInt();
            
            System.out.print("Ingrese el Tiempo (Segundos): ");
            int t = sc.nextInt();
                  
            int d = (v * t);
            System.out.println("Distancia: " + d);
            sc.close();  
      }  
}
```

_JOptionPane_

```
package ej01;

//Se reorganizo el codigo
import javax.swing.JOptionPane;

public class Ej01 {
	
      public static void main(String[] args) {
    	
        int v = Integer.parseInt(JOptionPane.showInputDialog(null, "Ingrese la Velocidad"));
        int t = Integer.parseInt(JOptionPane.showInputDialog(null, "Ingrese el Tiempo (Seg)"));
        
        int d = (v * t);  
        JOptionPane.showMessageDialog(null, "Distancia: " + d);    
      }
}
```

### Ejercicio 02
Calcula el promedio del estud.

_Sin Ingreso Por Teclado_

```
package ej02;
//Se reorganizo el codigo
public class Ej02 {

      public static void main (String [] args) {
      
      float n1=5;
      float n2=2;
      float n3=9;

      float prom=((n1+n2+n3)/3);
      System.out.print("Promedio: "+prom);
      }
}
```

_Scanner_ 

```
package ej02;
//Se reorganizo el codigo
import java.util.Scanner;

public class Ej02 {

      public static void main (String [] args) {

            Scanner sc=new Scanner(System.in); 

            float n1=sc.nextFloat();
            float n2=sc.nextFloat();
            float n3=sc.nextFloat();
            System.out.print("Ingrese las Calificaciones del Estud.");
            
            prom=((n1+n2+n3)/3)
            System.out.print("Promedio: "+prom);
      }
}
```

### Ejercicio 03
Calcula el puntaje de un equipo según los resultados de sus partidos. 

**Nota:** Los partidos ganados equivalen a 3 puntos, los partidos empatados equivalen a 1 punto y Los partidos perdidos equivalen a 0 puntos.

_Sin Ingreso Por Teclado_  

```
package ej03;
//Se reorganizo el codigo
public class Ej03 {

      public static void main (String [] args) {

            int puntaje=0;
            int pg=5;
            int pp=3;
            int pe=2;
      
            puntaje=(pg*3)+(pp*0)+(pe*1);
            System.out.print("Puntaje: "+puntaje);
      }
}
```

_Scanner_  

```
package ej03;

import java.util.Scanner;

public class Ej03 {

      public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int puntaje = 0;

        System.out.print("Ingrese el valor de pg: ");
        int pg = sc.nextInt();
        System.out.print("Ingrese el valor de pp: ");
        int pp = sc.nextInt();
        System.out.print("Ingrese el valor de pe: ");
        int pe = sc.nextInt();

        puntaje = (pg * 3) + (pp * 0) + (pe * 1);
        System.out.print("Puntaje: " + puntaje);    
      }
}
```

_JOptionPane_   

```
package ej03;

import javax.swing.JOptionPane;

public class Ej03 {

      public static void main(String[] args) {

            int puntaje = 0;

            String pgInput = JOptionPane.showInputDialog("Ingrese el valor de pg:");
            int pg = Integer.parseInt(pgInput);

            String ppInput = JOptionPane.showInputDialog("Ingrese el valor de pp:");
            int pp = Integer.parseInt(ppInput);

            String peInput = JOptionPane.showInputDialog("Ingrese el valor de pe:");
            int pe = Integer.parseInt(peInput);

            puntaje = (pg * 3) + (pp * 0) + (pe * 1);
            JOptionPane.showMessageDialog(null, "Puntaje: " + puntaje);
      }
}
```

### Ejercicio 04
Se debe identificar el día de la semana según el número. 

_Scanner_

```
package ej04;
//Se reorganizo el codigo
import java.util.Scanner;

public class Ej04 {

      public static void main(String[] args) {

            Scanner sc = new Scanner(System.in);
            float num = sc.nextFloat();

            if (num == 1) {
                  System.out.print("Lunes");
            } else if (num == 2) {
                  System.out.print("Martes");
            } else if (num == 3) {
                  System.out.print("Miércoles");
            } else if (num == 4) {
                  System.out.print("Jueves");
            } else if (num == 5) {
                  System.out.print("Viernes");
            } else if (num == 6) {
                  System.out.print("Sábado");
            } else if (num == 7) {
                  System.out.print("Domingo");
            } else {
                  System.out.print("!ERROR!");
                  System.out.print("No coincide con un día de la semana");
            }
      }
}
```

_JOptionPane_   

```
package ej04;

import javax.swing.JOptionPane;

public class Ej04 {

      public static void main(String[] args) {

            String numInput = JOptionPane.showInputDialog("Ingrese un número:");
            int num = Integer.parseInt(numInput);

            String mensaje = "";

            switch (num) {
                  case 1:
                  mensaje = "Lunes";
                  break;

                  case 2:
                  mensaje = "Martes";
                  break;

                  case 3:
                  mensaje = "Miércoles";
                  break;

                  case 4:
                  mensaje = "Jueves";
                  break;

                  case 5:
                  mensaje = "Viernes";
                  break;

                  case 6:
                  mensaje = "Sábado";
                  break;

                  case 7:
                  mensaje = "Domingo";
                  break;

                  default:
                  mensaje = "!ERROR!\n No coincide con un día de la semana";
                  break;
            }
            
            JOptionPane.showMessageDialog(null, mensaje);
      }
}
```

### Ejercicio 05
Convierta un valor dado en pesos colombianos a dolares. 

_Scanner_  

```
package ej05;
//Se reorganizo el codigo
import java.util.Scanner;

public class Ej05 {

      public static void main(String[] args) {
            
            Scanner sc = new Scanner(System.in);
            System.out.print("Conversor de Monto");
            System.out.print("Monto (Pesos Colombianos):");
            double valor = sc.nextDouble();

            double dolar = valor / 19.5; 
            System.out.print("Monto (Dólares): " + dolar);
      }
}
```

_JOptionPane_   

```
import javax.swing.JOptionPane;

public class Ej05 {

      public static void main(String[] args) {

            JOptionPane.showMessageDialog(null, "Conversor de Monto");

            String valorInput = JOptionPane.showInputDialog("Monto (Pesos Colombianos):");
            double valor = Double.parseDouble(valorInput);

            double dolar = valor / 19.5;

            JOptionPane.showMessageDialog(null, "Monto (Dólares): " + dolar);
      }
}
```


### Ejercicio 06
Menú con 5 opciones (If). 

_Scanner_

```
package ej06
import java.util.Scanner;
public class Ej06 {
      public static void main (String [] args) {
      Scanner sc=new Scanner(System.in);
      float num=sc.nextFloat();

      System.out.print("MENÚ");
      System.out.print("Ingrese un Digito (1 al 5)");

      if (dig==1){
      System.out.print("Conversor de Monto");
      System.out.print("Monto (Pesos Colombianos):");
      double valor=sc.nextDouble();
      dolar=((valor)/19.5);
      System.out.print("Monto (Dolares): "+dolar);
      }

      else if (dig==2){
      System.out.print("Calculadora de Promedios");
      System.out.print("Ingrese las Calificaciones del Estud.");
      float n1=sc.nextFloat();
      float n2=sc.nextFloat();
      float n3=sc.nextFloat();
      prom=((n1+n2+n3)/3);
      System.out.print("Promedio: "+prom);
      }
      
      else if (dig==3){
      System.out.print("Puntaje del Equipo A");
      int puntaje=0;
      int pg=5;
      int pp=3;
      int pe=2;
      puntaje=(pg*3)+(pp*0)+(pe*1);
      System.out.print("Puntaje: "+puntaje);
      }

      else if (dig==4){
      System.out.print("Verificador de Pares o Impares");
      System.out.print("Digite un Número");
      int num=sc.nextInt();
      if (num%2==0){
      System.out.print("Par");
      }
      else if (num%2!=0){
      System.out.print("Impar");
      }
      }

      else if (dig==5){
      System.out.print("Salir");
      }

      else {
      System.out.print("¡Error!");
      System.out.print("No existe dicha opción");
      }

}
```

### Ejercicio 06
Menú con 5 opciones (While/Switch). 

_Scanner_

```
package ej06
import java.util.Scanner;
public class Ej06 {
      public static void main (String [] args) {
      Scanner sc=new Scanner(System.in);
      int opcion=0;
      while(opcion!=5){
      System.out.print("MENÚ");
      System.out.print("1 (Conversor de Monto)");
      System.out.print("2 (Calculadora de Promedios)");
      System.out.print("3 (Puntaje del Equipo)");
      System.out.print("4 (Verificador de Pares o Impares)");
      System.out.print("5 (Salir)");
      }

      opcion=sc.nextInt();
      switch(opcion){
      case 1:
            System.out.print("Conversor de Monto");
            System.out.print("Monto (Pesos Colombianos):");
            double valor=sc.nextDouble();
            dolar=((valor)/19.5);
            System.out.print("Monto (Dolares): "+dolar);
            break;

      case 2:
            System.out.print("Calculadora de Promedios");
            System.out.print("Ingrese las Calificaciones del Estud.");
            float n1=sc.nextFloat();
            float n2=sc.nextFloat();
            float n3=sc.nextFloat();
            prom=((n1+n2+n3)/3);
            System.out.print("Promedio: "+prom);
            break;

      case 3:
            System.out.print("Puntaje del Equipo");
            int puntaje=0;
            int pg=5;
            int pp=3;
            int pe=2;
            puntaje=(pg*3)+(pp*0)+(pe*1);
            System.out.print("Puntaje: "+puntaje);
            break;
      
       case 4:
            System.out.print("Verificador de Pares o Impares");
            System.out.print("Digite un Número");
            int num=sc.nextInt();
            if (num%2==0){
            System.out.print("Par");
            }
            else if (num%2!=0){
            System.out.print("Impar");
            }
            break;
      
     case 5:
            System.out.print("Salir");
            break;

     default:
            System.out.print("¡Error!");
            System.out.print("No existe dicha opción");
            break;
            }

      }

}
```

### Ejercicio 07
Imprima la tabla del número 8.

_Sin Ingreso Por Teclado_

```
package ej07

public class Ej07 {
      public static void main (String [] args) {
      
      	int num=8;
      	int multiplo=0;

      	for (int i=0; i<11; i++){
		multiplo=(num*i);
		System.out.print("8 x "+ i +"= "+multiplo);
      	}
}
```

### Ejercicio 08
Suma Continua.

_Sin Ingreso Por Teclado_

```
package ej08

public class Ej08 {
      public static void main (String [] args) {

      	int a=1;
      	int b=0;
      	int n=20;

	for (int i=0; i<11; i++){
      		int suma=a+b;
      		System.out.print(suma+ i +" ");
      		a=b;
      		b=suma;
      	}
}
```

### Ejercicio 09
Menú con 3 opciones (While/Switch). 

_Scanner_

```
package ej09
import java.util.Scanner;
public class Ej09 {
      public static void main (String [] args) {
      Scanner sc=new Scanner(System.in);
      int opcion=0;
      while(opcion!=3){
            System.out.print("MENU\n");
		System.out.print("Elija Una Opción\n"); 
		System.out.print("1 Suma\n"); 
		System.out.print("2 Promedio\n"); 
		System.out.print("3 Salida\n"); 
      

      opcion=sc.nextInt();
      switch(opcion){
      case 1:
            int suma=0;
            int num=-1;
                  while (num!=0){
                  System.out.print("Digite Un Número Entero (Digite 0 Para Terminar)");
                  num=sc.nextInt();
                  suma+=num;
                  }
            System.out.print(suma+" :Resultado");
            break;

      case 2:
            System.out.print("Ingrese 10 Números");
            int numero=10;
            int adicion=0;
                  for (int i=1; i<=numero; ++){
                  int numero=sc.nextInt();
                  adicion+=numero;
                  }
            double prom=(double) adicion/numero;
            System.out.print(prom+" :Promedio");
            break;

      case 3:
            System.out.print("Salir");
            break;

     default:
            System.out.print("¡Error!");
            System.out.print("No existe dicha opción");
            break;
            }

      }

}
```

_JOptionPane_

```
package ej09
import javax.swing.JOptionPane;
public class Ej09 {
      public static void main (String [] args) {
      Scanner sc=new Scanner(System.in);
      int opcion=0;
      while(opcion!=3){
      JOptionPane.showMessageDialog(null, "MENÚ");
      opcion=Integer.parseInt(JOptionPane.showInputDialog(null, "Digite Una Opción"));

      switch(opcion){
      case 1:
            JOptionPane.showMessageDialog(null, "Opción 01: Suma");
            int suma=0;
            int num=-1;
                  while (num!=0){
                  num=Integer.parseInt(JOptionPane.showInputDialog(null, "Digite Un Número Entero (Digite 0 Para Terminar)"));
                  suma+=num;
                  }
            JOptionPane.showMessageDialog(null, suma+" :Resultado");
            break;

      case 2:
            JOptionPane.showMessageDialog(null, "Opción 02: Calcular Promedio");
            int numeros=10;
            int adicion=0;
                  for (int i=1; i<=numero; ++){
                  int numero=Integer.parseInt(JOptionPane.showInputDialog(null, "Digite 10 Números"));
                  adicion+=numero;
                  }
            double prom=(double) adicion/numeros;
            JOptionPane.showMessageDialog(null, prom+" :Resultado");
            break;

      case 3:
            JOptionPane.showMessageDialog(null, "Salir");
            break;

     default:
            JOptionPane.showMessageDialog(null, "¡Error!");
            JOptionPane.showMessageDialog(null, "No existe dicha opción");
            break;
            }

      }

}
```

### Ejercicio 10
Imprime un Mensaje. 

_JOptionPane_

```
package ej10
import javax.swing.JOptionPane;
public class Ej10 {
      public static void main (String [] args) {
      JOptionPane.showMessageDialog(null, "LOL");
      }
}
```

### Ejercicio 11
Introduce tu Nombre. 

_JOptionPane_

```
package ej11
import javax.swing.JOptionPane;
public class Ej11 {
      public static void main (String [] args) {
      String name=JOptionPane.showInputDialog(null, "Introduce tu Nombre. Por Favor");
      JOptionPane.showMessageDialog(null, name);
      }
}
```

### Ejercicio 12
Calculadora Básica. 

_JOptionPane_

```
package ej12

import javax.swing.JOptionPane;

public class Ej12 {

      public static void main (String [] args) {

            int x = Integer.ParseInt(JOptionPane.showInputDialog(null, "Digite Un Número"));
            int y = Integer.ParseInt(JOptionPane.showInputDialog(null, "Digite Un Número"));

            int a = suma(x, y);
            JOptionPane.showMessageDialog(null, "SUMA: " + a);

            int b = resta(x, y);
            JOptionPane.showMessageDialog(null, "RESTA: " + b);

            int c = multiplicacion(x, y);
            JOptionPane.showMessageDialog(null, "MULTIPLICACIÓN: " + c);

            int d = division(x, y);
            JOptionPane.showMessageDialog(null, "DIVISIÓN: " + d);
      }

      public static int suma(int x, int y) {
            return (x + y);
       }
      

      public static int resta(int x, int y) {
            return (x - y);
      }

      public static int multiplicacion(int x, int y) {
            return (x * y);
      }

      public static int division(int x, int y) {
            return (x / y);
      }
}
```

### Ejercicio 13
Introduce tu Nombre. 

_JOptionPane_

```
package ej13;
//Se reorganizo el codigo
import javax.swing.JOptionPane;

public class Ej13 {

      public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Cálculo de Factorial");
        JOptionPane.showMessageDialog(null, "Advertencia\n Ingrese Solo Números Enteros Positivos");

        boolean continuar = true;

        while (continuar) {
            String input = JOptionPane.showInputDialog("Digite Un Número:");
            int numero;

            if (input != null && input.matches("\\d+")) {
                  numero = Integer.parseInt(input);

                  if (numero >= 0) {
                        long factorial = calcularFactorial(numero);
                        JOptionPane.showMessageDialog(null, "El factorial de " + numero + " es " + factorial);
                  } else {
                        JOptionPane.showMessageDialog(null, "¡ERROR!\n Por favor, Ingrese un Número Entero Positivo.");
                  }

            } else {
                  JOptionPane.showMessageDialog(null, "¡ERROR!. Por Favor, Ingrese un Número Entero Positivo.");
                  continue;
            }

            String respuesta = JOptionPane.showInputDialog("¿Desea Calcular el Factorial de Otro Número?\n (Sí/No)").toLowerCase();
            if (!respuesta.equals("sí")) {
                continuar = false;
            }
        }
      }

    public static long calcularFactorial(int numero) {
      if (numero <= 1) {
            return 1;
      } else {
            return numero * calcularFactorial(numero - 1);
      }
    }
}
```

### Ejercicio 14
Muestra la nota maxíma o mínima del estud. 

_JOptionPane_

```
package ej14;

import javax.swing.JOptionPane;

public class Ej14 {

      public static void main(String[] args) {
        int lim = Integer.parseInt(JOptionPane.showInputDialog(null, "Ingrese el No. de Calificaciones"));
        int num[] = new int[lim];
        double suma = 0;

        for (int i = 0; i < lim; i++) {
            num[i] = Integer.parseInt(JOptionPane.showInputDialog(null, "Ingrese Calificación del Estud.\n"));
            suma += num[i];
        }

        int max = num[0]; 
        int min = num[0]; 

        for (int i = 1; i < lim; i++) {
            if (num[i] > max) {
                  max = num[i];
            }
            if (num[i] < min) {
                  min = num[i];
            }
        }

        double prom = (suma / lim); 

        JOptionPane.showMessageDialog(null, "Nota Máxima: " + max + "\n" + "Nota Mínima: " + min + "\n" + "Promedio: " + prom);
      }
}
```

### Ejercicio 15
Calcular promedio del estud. (Try-Catch) 

_JOptionPane_

```
package ej15;

import javax.swing.JOptionPane;

public class Ej15 {

	public static void main(String[] args) {
		
		JOptionPane.showMessageDialog(null, "Ponderación del Estud.");
		
		float [] nota=new float [3];
		double suma=0;
		double prom=0;
		
		for (int i=0; i<3; i++) {
			try {
			    nota[i] = Float.parseFloat(JOptionPane.showInputDialog(null, "Calificación " + (i+1)));
			    suma+=nota[i];
			} catch (NumberFormatException e) {
			    JOptionPane.showMessageDialog(null, "¡ERROR!\n Ingrese Un Número\n (Entero o Decimal)");
			    i--;
			}
		}
		
		prom=suma/3;
		JOptionPane.showMessageDialog(null, "Promedio: "+ prom); 
	}
}
```

## Despliegue (Deployment)

Serie de ejercicios desarrollados en eclipse a lo largo del segundo semestre, 
cuya tematica fue impartida por el docente a cargo de la asignatura "Mauricio Lopéz" 
al cual se le otorga su debido agradecimiento.

## Construido con

Eclipse: Programa de Desarrollo Java.

## Versionado

Eclipse (Versión 2022-12).

## Autor(es)

Juan Eraso, Jaider Narvaèz.

## Expresiones de gratitud (Acknowledgments)

* Aprende de poco a poco para llegar lejos...
