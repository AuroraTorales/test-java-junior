String letra = "6";
    String prefijo = "Iteracion nro ";
    for (int i = 0; i < 10; i++) {
        if (letra == String.valueOf(i)) {
            System.out.println("El bucle continua");
            break;
        } else {
            System.out.println(prefijo + i);
        }
    }

Resultado: 
Iteracion nro 0
Iteracion nro 1
Iteracion nro 2
Iteracion nro 3
Iteracion nro 4
Iteracion nro 5
Iteracion nro 6
Iteracion nro 7
Iteracion nro 8
Iteracion nro 9

Explicación: Realiza la segunda condición porque la primera condición la comparación no puede ser dada, el == se utiliza para comparar
a nivel de Objeto, determina si ambos objetos en sí son iguales. En este caso para que la primera condición se ejecute
se debe cambiar el "==" por el equals, éste compara los caracteres dentro del objeto String por ende de ese modo se 
puede ejecutar el primer if.
	Quedaría así:
String letra = "6";
    String prefijo = "Iteracion nro ";
    for (int i = 0; i < 10; i++) {
        if (letra.equals(String.valueOf(i))) {
            System.out.println("El bucle continua");
            break; //Indica que el for finaliza 
        } else {
            System.out.println(prefijo + i);
        }
    }
Resultado:

Iteracion nro 0
Iteracion nro 1
Iteracion nro 2
Iteracion nro 3
Iteracion nro 4
Iteracion nro 5
El bucle continua
