This is my First Repository
<br>
Author - Vidhi Sontakke


```java

import java.util.Scanner;
import java.util.Random;

class GuessGame {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

        int computerNumber = rand.nextInt(100) + 1;
        int guess;
        int chances = 5;

        System.out.println(" Guess the Number Game");
        System.out.println("You have 5 chances to guess a number between 1 to 100");

        for (int i = 1; i <= chances; i++) {
            System.out.print("Chance " + i + " - Enter your guess: ");
            guess = sc.nextInt();

            if (guess == computerNumber) {
                System.out.println(" Correct! You Win.");
                break;
            } 
            else if (guess > computerNumber) {
                System.out.println("Too High");
            } 
            else {
                System.out.println("Too Low");
            }

            if (i == chances) {
                System.out.println("Game Over!");
                System.out.println("Correct number was: " + computerNumber);
            }
        }
    }
}



