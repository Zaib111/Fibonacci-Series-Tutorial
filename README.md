import java.util.Scanner;
//Purpose: To create a program that outputs a custom fibonacci sequence, based on the first two numbers in the sequence that the user will provide.

class Main {
  public static void main(String[] args) {
    Scanner input = new Scanner(System.in);
    
    System.out.print("Enter the first number: ");
    int firstNumber = input.nextInt();

    System.out.print("Enter the second number: ");
    int secondNumber = input.nextInt();

    System.out.print("Enter the number of terms in the series: ");
    int numberOfTerms = input.nextInt();

    System.out.println("\nFibonacci Series:");
    System.out.print(firstNumber + ", " + secondNumber);

    for(int i=2;i<numberOfTerms;i++){
      int nextNumber = firstNumber + secondNumber;
      System.out.print(", " + nextNumber);
      firstNumber = secondNumber;
      secondNumber = nextNumber;

    }
      
  }
}
