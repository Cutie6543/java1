# java1
import java.util.Scanner;
 class GradeCalculator {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Define weights for each component
        double assignmentWeight = 0.4;
        double quizWeight = 0.2;
        double examWeight = 0.4;

        // Get grades for each component
        System.out.print("Enter the grade for assignments (0-100): ");
        double assignmentGrade = scanner.nextDouble();

        System.out.print("Enter the grade for quizzes (0-100): ");
        double quizGrade = scanner.nextDouble();

        System.out.print("Enter the grade for exams (0-100): ");
        double examGrade = scanner.nextDouble();

        // Calculate the final grade
        double finalGrade = (assignmentGrade * assignmentWeight) +
                            (quizGrade * quizWeight) +
                            (examGrade * examWeight);

        // Print the final grade
        System.out.printf("The final grade is: %.2f%n", finalGrade);

        scanner.close();
    }
}

program on student grade calculator
