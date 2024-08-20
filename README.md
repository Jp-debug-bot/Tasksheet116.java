# Tasksheet116.java
import java.util.*;

public class PalindromeChecker {

    public static void main(String[] args) {
        // Create a Scanner object to read input from the user
        Scanner scanner = new Scanner(System.in);

        // Ask the user to enter a string
        System.out.println("Enter a string:");
        String inputString = scanner.nextLine();

        // Use StringBuilder to create a reverse of the input string
        StringBuilder reversedString = new StringBuilder(inputString);
        reversedString.reverse();

        // Check if the input string and the reversed string are the same
        if (inputString.equals(reversedString.toString())) {
            System.out.println("The input string is a palindrome.");
        } else {
            System.out.println("The input string is not a palindrome.");
        }

        // Close the scanner
        scanner.close();
    }
}
