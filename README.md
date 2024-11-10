# seany-
1. Calculadora de Calificaciones Finales
java

import java.util.Scanner;

public class CalculadoraCalificaciones {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir calificaciones
        System.out.print("Ingrese la calificación del primer parcial: ");
        double parcial1 = scanner.nextDouble();

        System.out.print("Ingrese la calificación del segundo parcial: ");
        double parcial2 = scanner.nextDouble();

        System.out.print("Ingrese la calificación del proyecto: ");
        double proyecto = scanner.nextDouble();

        System.out.print("Ingrese la calificación del examen final: ");
        double examenFinal = scanner.nextDouble();

        // Verificar si las calificaciones están en el rango adecuado
        if (parcial1 < 0 || parcial1 > 100 || parcial2 < 0 || parcial2 > 100 || 
            proyecto < 0 || proyecto > 100 || examenFinal < 0 || examenFinal > 100) {
            System.out.println("Las calificaciones deben estar entre 0 y 100.");
            return;
        }

        // Calcular la nota final
        double notaFinal = (parcial1 + parcial2) * 0.4 / 2 + proyecto * 0.3 + examenFinal * 0.3;
        System.out.println("La calificación final es: " + notaFinal);
    }
}







2. Verificar Edad para Votar
java
import java.util.Scanner;

public class VerificarEdad {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir la edad
        System.out.print("Ingrese su edad: ");
        int edad = scanner.nextInt();

        // Verificar si puede votar
        if (edad >= 18) {
            System.out.println("Usted es elegible para votar.");
        } else {
            System.out.println("Usted no es elegible para votar.");
        3. Evaluación de Calificaciones con Letras
java

import java.util.Scanner;

public class EvaluacionCalificaciones {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir calificación numérica
        System.out.print("Ingrese su calificación: ");
        double calificacion = scanner.nextDouble();

        // Evaluar la calificación
        char letra;
        if (calificacion >= 90 && calificacion <= 100) {
            letra = 'A';
        } else if (calificacion >= 80) {
            letra = 'B';
        } else if (calificacion >= 70) {
            letra = 'C';
        } else if (calificacion >= 60) {
            letra = 'D';
        } else {
            letra = 'F';
        }

        // Imprimir la letra correspondiente
        System.out.println("Su calificación es: " + letra);
    
________________________________________

4. Calcular Precio con Descuento
java
import java.util.Scanner;

public class PrecioConDescuento {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir precio del producto
        System.out.print("Ingrese el precio del producto: ");
        double precio = scanner.nextDouble();

        // Calcular descuento
        double descuento = 0;
        if (precio > 100 && precio <= 200) {
            descuento = 0.1;
        } else if (precio > 200 && precio <= 500) {
            descuento = 0.2;
        } else if (precio > 500) {
            descuento = 0.25;
        }

        double precioFinal = precio - (precio * descuento);
        System.out.println("El precio final con descuento es: " + precioFinal);
    

5. Determinar la Estación del Año
java
import java.util.Scanner;

public class EstacionDelAño {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir mes
        System.out.print("Ingrese el número del mes (1-12): ");
        int mes = scanner.nextInt();

        // Determinar estación del año
        String estacion;
        switch (mes) {
            case 12: case 1: case 2:
                estacion = "Invierno";
                break;
            case 3: case 4: case 5:
                estacion = "Primavera";
                break;
            case 6: case 7: case 8:
                estacion = "Verano";
                break;
            case 9: case 10: case 11:
                estacion = "Otoño";
                break;
            default:
                estacion = "Mes inválido";
        }

        System.out.println("La estación es: " + estacion);
 

6. Convertidor de Grados
java
import java.util.Scanner;

public class ConvertidorDeGrados {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir temperatura en Celsius
        System.out.print("Ingrese la temperatura en grados Celsius: ");
        double celsius = scanner.nextDouble();

        // Menú para elegir conversión
        System.out.println("Seleccione una opción:");
        System.out.println("1. Convertir a Fahrenheit");
        System.out.println("2. Convertir a Kelvin");
        int opcion = scanner.nextInt();

        // Realizar conversión
        double resultado;
        switch (opcion) {
            case 1:
                resultado = (celsius * 9/5) + 32;
                System.out.println("La temperatura en Fahrenheit es: " + resultado);
                break;
            case 2:
                resultado = celsius + 273.15;
                System.out.println("La temperatura en Kelvin es: " + resultado);
                break;
            default:
                System.out.println("Opción inválida.");
       


7. Conversor de Monedas
java

import java.util.Scanner;

public class ConversorDeMonedas {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir monto en pesos mexicanos
        System.out.print("Ingrese la cantidad en pesos mexicanos: ");
        double pesos = scanner.nextDouble();

        // Menú de monedas
        System.out.println("Seleccione la moneda a convertir:");
        System.out.println("1. Dólar (USD)");
        System.out.println("2. Euro (EUR)");
        System.out.println("3. Bath (THB)");
        System.out.println("4. Yen (JPY)");
        System.out.println("5. Won (KRW)");
        System.out.println("6. Dólar Australiano (AUD)");
        System.out.println("7. Sol (PEN)");
        System.out.println("8. Dólar Canadiense (CAD)");
        System.out.println("9. Bolívar (VES)");
        System.out.println("10. Peso Argentino (ARS)");
        int opcion = scanner.nextInt();

        // Realizar conversión
        double resultado;
        switch (opcion) {
            case 1:
                resultado = pesos * 0.058;
                System.out.println("Cantidad en USD: " + resultado);
                break;
            case 2:
                resultado = pesos * 0.054;
                System.out.println("Cantidad en EUR: " + resultado);
                break;
            case 3:
                resultado = pesos * 2.08;
                System.out.println("Cantidad en THB: " + resultado);
                break;
            case 4:
                resultado = pesos * 7.9;
                System.out.println("Cantidad en JPY: " + resultado);
                break;
            case 5:
                resultado = pesos * 79.5;
                System.out.println("Cantidad en KRW: " + resultado);
                break;
            case 6:
                resultado = pesos * 0.089;
                System.out.println("Cantidad en AUD: " + resultado);
                break;
            case 7:
                resultado = pesos * 0.22;
                System.out.println("Cantidad en PEN: " + resultado);
                break;
            case 8:
                resultado = pesos * 0.078;
                System.out.println("Cantidad en CAD: " + resultado);
                break;
            case 9:
                resultado = pesos * 1.8;
                System.out.println("Cantidad en VES: " + resultado);
                break;
            case 10:
                resultado = pesos * 15.6;
                System.out.println("Cantidad en ARS: " + resultado);
                break;
            default:
                System.out.println("Opción inválida.");

8. Brindar Información
java

import java.util.Scanner;

public class BrindarInformacion {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir entrada de usuario
        System.out.print("Ingrese el nombre de un artista, película, serie o algo de su preferencia: ");
        String eleccion = scanner.nextLine();

        // Brindar información usando switch
        switch (eleccion.toLowerCase()) {
            case "chicago":
                System.out.println("Chicago es una famosa película de 2002 basada en el musical homónimo.");
                break;
            case "da vinci":
                System.out.println("Leonardo da Vinci fue un renombrado artista y científico italiano.");
                break;
            case "game of thrones":
                System.out.println("Game of Thrones es una serie de televisión basada en los libros de George R.R. Martin.");
                break;
            case "the beatles":
                System.out.println("The Beatles es una de las bandas más famosas de la historia del rock.");
                break;
            case "avatar":
                System.out.println("Avatar es una película de ciencia ficción dirigida por James Cameron.");
                break;
            default:
                      
