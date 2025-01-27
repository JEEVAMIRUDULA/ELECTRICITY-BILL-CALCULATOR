# ELECTRICITY-BILL-CALCULATOR
import java.util.Scanner;

public class ElectricBillCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of units consumed: ");
        int units = scanner.nextInt(); 
        double rate; 
        double bill; 
        if (units <= 100) {
            rate = 1.0; // Rate per unit for <= 100 units
        } else if (units <= 300) {
            rate = 1.5; // Rate per unit for 101-300 units
        } else {
            rate = 2.0; // Rate per unit for > 300 units
        }

        bill = units * rate;
        System.out.println("The total electricity bill is: " + bill);

        scanner.close(); 

    }
}
 O/P

Enter the number of units consumed: 350
The total electricity bill is: 700.0

