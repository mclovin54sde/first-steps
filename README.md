# first-steps
these are my first code blocks as a newbie 
import java.util.Scanner;

class B {
    public static void main(String args[]) {
        int a = 100;
        int b = 10;
        int c;
        Scanner sc = new Scanner(System.in);

        while (a > b) {
            System.out.println("Enter a value for c (or enter a value greater than 100 to exit):");
            c = sc.nextInt(); // Read new input each iteration

            if (c < a) {
                System.out.println("c is less than a");
            } else {
                System.out.println("c is not lesser than a");
            }

            // Provide an exit condition
            if (c > 100) {
                System.out.println("Exiting the loop as c > 100.");
                break;
            }
        }

        sc.close(); // Close the scanner resource
    }
}
