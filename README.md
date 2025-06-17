import java.util.Scanner;

public class Calculator {
  public static void main(String[] args) {
    Scanner input = new Scanner(System.in);
    System.out.println("Enter two numbers:");
    double a = input.nextDouble();
    double b = input.nextDouble();
    
    System.out.println("Enter operation (+, -, *, /):");
    char op = input.next().charAt(0);
    
    double result = 0;
    switch (op) {
      case '+': result = a + b; break;
      case '-': result = a - b; break;
      case '*': result = a * b; break;
      case '/': result = a / b; break;
      default: System.out.println("Invalid operator!");
    }

    System.out.println("Result: " + result);
  }
}
