# Calculator

package calculator;

import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		
		double number1, number2, result;
        char choose;
		Scanner input = new Scanner(System.in);
		
		System.out.println("Enter the first number:");
	    number1 = input.nextDouble();
		
		System.out.println("Enter the second number: ");
	    number2 = input.nextDouble();
	     
	     System.out.println("1.Multiplication");
	     System.out.println("2.Extraction");
	     System.out.println("3.Multiplication");
	     System.out.println("4.Division");
	     System.out.println("Choose the operation: ");
	     choose = input.next().charAt(0);
	     
	switch(choose){
      case '1':
	     result = number1 + number2;
	     System.out.println("Result:" +result);
	     break;
	     
      case '2':
         result = number1 - number2;
         System.out.println("Result:" +result);
	     break;
	     
      case '3':
        result = number1 * number2;
        System.out.println("Result:" +result);
        break; 
        
      case '4':
        if (number2 == 0) {
        	System.out.println("This number cannot divide by zero.");
        break;
        }
        else {
        	result = number1/number2;
        	System.out.println("Result:" +result);
            break;
        }
      default:
          System.out.print("Choose one of those operations.");
          break;
      
	
	   }	

	}

}
