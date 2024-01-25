import java.util.Scanner;

public class Studentgradecalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the number of subjects: ");
        int numSubjects = scanner.nextInt();

        int totalMarks = 0;

        for (int i = 1; i <= numSubjects; i++) {
            System.out.print("Enter marks for Subject " + i + ": ");
            int marks = scanner.nextInt();
            totalMarks += marks;
        }

        double averagePercentage = (double) totalMarks / numSubjects;

        char grade = calculateGrade(averagePercentage);

        System.out.println("\nTotal Marks: " + totalMarks);
        System.out.println("Average Percentage: " + averagePercentage + "%");
        System.out.println("Grade: " + grade);

        scanner.close();
    }

    private static char calculateGrade(double averagePercentage) {
       
        if (averagePercentage >= 90)
         {
            return 'O';
        }
         else if (averagePercentage >= 80)
          {
            return 'A';
        } 
        else if (averagePercentage >= 70) 
        {
            return 'B';
        }
         else if (averagePercentage >= 60) 
         {
            return 'C';
        } 
        else if (averagePercentage >= 50)
        {
            return 'D';
        }
        else if (averagePercentage >= 40)
        {
            return 'P';
        }
        else {
            return 'F';
        }
    }
}
