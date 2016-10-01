# Min-Max-Avg

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        int high = -1000000;
        int low = 100000;
        int number;
        int count = 0;
        long total = 0;
        double avg = 0.0;
        boolean loop = true;
        Scanner input = new Scanner(System.in);
        while (loop) {

            do {
                System.out.println("Please enter a number");
                number = input.nextInt();
            } while ((number < -1000000) || (number > 1000000));
            count++;
                total += number;
                avg = total/count;
            if (number < low) {
                low = number;
            }

            if (number > high) {
                high = number;
            }

            System.out.println(low);
            System.out.println(high);
            System.out.println(avg);

        }

    }
}
