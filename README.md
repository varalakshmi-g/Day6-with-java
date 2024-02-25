# Day6-with-java

Successfully completed day 5 at #30DaysCodeAtTAPAcademy also it was my day 6 of my coding challenge.

Today's challenge is to Write a program that takes two integers, n1 and n2, as input and prints the first y common multiples of n1 and n2.



here is the solution



import java.util.Scanner;



public class CommonMultiples {

  public static void main(String[] args) {

    Scanner scan = new Scanner(System.in);



    System.out.print("Enter the first integer n1: ");

    int n1 = scan.nextInt();



    System.out.print("Enter the second integer n2: ");

    int n2 = scan.nextInt();



    System.out.print("Enter the number of common multiples to print y: ");

    int y = scan.nextInt();



    int smallestN1 = (int) Math.ceil((double) Math.max(n1, n2) / Math.min(n1, n2));



    for (int i = 0; i < y; i++) {

      System.out.println("Common multiple " + (i + 1) + ": " + (smallestN1 * n2));

      smallestN1++;

    }



    scan.close();

  }

}

