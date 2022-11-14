# Program-to-cast-alphabets-to-their-ASCII-Code
    1. Write a program that prompts the user to input an integer between 0 and 35. If the number is less than or equal to 9, the program should output the number; otherwise, it should output A for 10, B for 11, C for 12, . . ., and Z for 35.  (Hint: Use the cast operator, (char)( ), for numbers >= 10.)


		Program-to-cast-alphabets-to-their-ASCII-Code



import java.util.Scanner;


public class Question1 {
    public static void main(String[] args) {


        Scanner console = new Scanner(System.in);

        System.out.print("Enter a number: ");

        int number = console.nextInt();

        if(number<=9){

            System.out.print(number);

        }else if (number>=10 || number<=35){

            int num = number+55;

            char character = (char) num;

            System.out.println(character);

        }

    }
}
