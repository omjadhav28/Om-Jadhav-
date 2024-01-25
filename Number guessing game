import java.util.Random;
import java.util.Scanner;

public class Numberguessinggame {

    private int totalCorrectGuesses = 0;

    public static void main(String[] args) {
        Numberguessinggame game = new Numberguessinggame();
        game.playGame();
    }

    public void guessNumber() {
        int minNumber = 1;
        int maxNumber = 100;

        Random random = new Random();
        int secretNumber = random.nextInt(maxNumber - minNumber + 1) + minNumber;

        int K = 5;
        int roundScore = 0;

        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to the Number Guessing Game!");
        System.out.println("I've picked a number between " + minNumber + " and " + maxNumber + ". Try to guess it.");

        while (K > 0) {
            int guess;
            try {
                System.out.print("Your guess: ");
                guess = scanner.nextInt();
            } catch (Exception e) {
                System.out.println("Please enter a valid number.");
                scanner.nextLine(); 
                continue;
            }

            K--;

            if (guess == secretNumber) {
                System.out.println("Congratulations! You've guessed the number " + secretNumber + "! It took you " + (5- K) + " attempts.");
                roundScore++;
                break;
            } else if (guess < secretNumber) {
                System.out.println("The Number is " + " Greater than "+guess);
            } else {
                System.out.println("The Number is " + " Smaller than "+guess);
            }
        }
        if (K == 0) {
            System.out.println(" you have Exahusted 5 Attempts");
            System.out.println("The number was "+ secretNumber);
            
        }

        System.out.println("Your score for this round: " + roundScore);
        totalCorrectGuesses += roundScore; 
    }

    public void playGame() {
        Scanner scanner = new Scanner(System.in);

        while (true) {
            guessNumber();

            System.out.print("Do you want to play again? (yes/no): ");
            String playAgain = scanner.next().toLowerCase();
            if (!playAgain.equals("yes")) {
                break;
            }
        }

        System.out.println("Thanks for playing! Total correct guesses: " + totalCorrectGuesses);
    }
}
