QUESTION 1 ; Write a program to print whether a number is even or odd, also take input from the user.

import java.util.*;
public class Main{
    public static void main(String args[]){
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        if(n % 2 == 0)
            System.out.println("Even");
        else
            System.out.println("Odd");
    }
}
OUTPUT ; 
Enter a number: 20
Even

QUESTION 2 ;Take name as input and print a greeting message for that particular name.

public class GreetingProgram {
    public static void main(String[] args) {
        java.io.Console console = System.console();

        if (console == null) {
            System.out.println("Console not available. Run via Terminal.");
            return;
        }

        String name = console.readLine("Please enter your name: ");

        System.out.println("Hello, " + name + "! Welcome and happy coding!");
    }
}
OUTPUT ;
Please enter your name: VAISHU
Hello, VAISHU! Welcome and happy coding!

QUESTION 3 ;Write a program to input principal, time, and rate (P, T, R) from the user and find Simple Interest.Take in two numbers and an operator (+, -, *, /) and calculate the value. (Use if conditions)

public class SimpleInterest {
    public static void main(String[] args) {
        java.io.Console console = System.console();

        if (console == null) {
            System.out.println("Console not available. Run via Terminal.");
            return;
        }

        double p = Double.parseDouble(console.readLine("Enter Principal (P): "));
        double t = Double.parseDouble(console.readLine("Enter Time in years (T): "));
        double r = Double.parseDouble(console.readLine("Enter Rate of Interest (R): "));

        double si = (p * t * r) / 100;

        System.out.println("Simple Interest = " + si);
    }
}
OUTPUT ;
Enter Principal (P): 10000
Enter Time in years (T): 2
Enter Rate of Interest (R): 4
Simple Interest = 800.0

QUESTION 4 ;Take in two numbers and an operator (+, -, *, /) and calculate the value. (Use if conditions)

public static void main(String[] args) {
        // Predefined inputs (Change these values to test different cases)
        double num1 = 10.5;
        double num2 = 2.5;
        char operator = '*'; // Supports: '+', '-', '*', '/'

        double result = 0;
        boolean validOperation = true;

        // Evaluation logic using if-else conditions
        if (operator == '+') {
            result = num1 + num2;
        } else if (operator == '-') {
            result = num1 - num2;
        } else if (operator == '*') {
            result = num1 * num2;
        } else if (operator == '/') {
            // Error handling for division by zero
            if (num2 != 0) {
                result = num1 / num2;
            } else {
                System.out.println("Error: Division by zero is not allowed.");
                validOperation = false;
            }
        } else {
            System.out.println("Error: Invalid operator entered.");
            validOperation = false;
        }

        // Print final output if the operation was successful
        if (validOperation) {
            System.out.println("Calculation: " + num1 + " " + operator + " " + num2 + " = " + result);
        }
    }
}
OUTPUT ;
Calculation: 10.5 * 2.5 = 26.25

QUESTION 5 ; 
Take 2 numbers as input and print the largest number.
import java.util.Scanner;

class Main
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        if(a > b)
            System.out.println("Largest number = " + a);
        else
            System.out.println("Largest number = " + b);
    }
}
OUTPUT ; 
Enter first number: 999
Enter second number: 1999
Largest number = 1999

QUESTION 6 ;
Input currency in rupees and output in USD.

import java.util.Scanner;

class Main
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter amount in Rupees: ");
        double rupees = sc.nextDouble();

        double usd = rupees / 86;

        System.out.println("USD = " + usd);
    }
}

OUTPUT ;
Enter amount in Rupees: 980
USD = 11.395348837209303

QUESTION 7 ;
To calculate Fibonacci Series up to n numbers.
import java.util.Scanner;

class Main
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter the number: ");
        int n = sc.nextInt();

        int a = 0, b = 1;

        System.out.print("Fibonacci Series: ");

        for(int i = 1; i <= n; i++)
        {
            System.out.print(a + " ");
            int c = a + b;
            a = b;
            b = c;
        }
    }
}
OUTPUT ;
Enter the number: 20
Fibonacci Series: 0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987 1597 2584 4181 
QUESTION 8 ;
To find out whether the given String is Palindrome or not.
import java.util.*;

class Main
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);

        String s = sc.next();
        String rev = new StringBuffer(s).reverse().toString();

        if(s.equals(rev))
            System.out.println("Palindrome");
        else
            System.out.println("Not Palindrome");
    }
}
