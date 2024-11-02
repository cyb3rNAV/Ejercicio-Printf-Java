# Ejercicio-Printf-Java
Aquí dejo un ejercicio para practicar el printf en Java ya que nos han dicho que cae si o si en el examen de programación de DAM 

EJERCICIO: Realiza un programa que calcule el perímetro y el área de un rectángulo. La longitud de los lados se introducirán por teclado.

El resultado se mostrará por pantalla y tendrá el siguiente formato:

"El rectangulo de lados <ancho> , <alto> tiene un perimetro = <valor_perímetro> y un area = <valor_área>"

SOLUCION:

import java.util.Scanner;
class Rectangulo {
    public static void main(String[] args) {
       Scanner scanner = new Scanner(System.in);
       
        System.out.print("Introduzca el ancho: ");
        
        double ancho = scanner.nextDouble();
        
        System.out.print("Introduzca la altura: ");
        
        double altura = scanner.nextDouble();
        
        double perimetro = 2 * (ancho + altura);
        
        double area = ancho * altura;
        
        System.out.printf("El rectangulo de %.2f y %.2f tiene un perimetro = %.2f y un area = %.2f%n", ancho, altura, perimetro, area);
