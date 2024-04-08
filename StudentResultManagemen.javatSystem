import java.util.Scanner;

public class StudentResult {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Input from user
        System.out.print("Enter student roll number: ");
        int rollNumber = scanner.nextInt();

        int[] marks = new int[5]; // Array to store marks for 5 subjects
        System.out.println("Enter marks for 5 subjects: ");
        for (int i = 0; i < marks.length; i++) {
            System.out.print("Subject " + (i + 1) + ": ");
            marks[i] = scanner.nextInt();
        }

        // Calculate total marks
        int totalMarks = 0;
        for (int mark : marks) {
            totalMarks += mark;
        }

        // Calculate percentage
        double percentage = (double) totalMarks * 100 / 500;

        // Calculate rank
        String rank = calculateRank(percentage);

        // Display results
        System.out.println("\nStudent Result:");
        System.out.println("Roll Number: " + rollNumber);
        System.out.println("---------------------");
        for (int i = 0; i < marks.length; i++) {
            System.out.println("Subject " + (i + 1) + " Marks: " + marks[i]);
        }
        System.out.println("Total Marks: " + totalMarks);
        System.out.println("Percentage: " + percentage + "%");
        System.out.println("Rank: " + rank);
    }

    // Method to calculate rank based on percentage
    public static String calculateRank(double percentage) {
        if (percentage >= 95) {
            return "A+";
        } else if (percentage >= 80) {
            return "A";
        } else if (percentage >= 70) {
            return "B+";
        } else if (percentage >= 60) {
            return "B";
        } else if (percentage >= 50) {
            return "C";
        } else if (percentage >= 40) {
            return "D";
        } else {
            return "FAIL";
        }
    }
}
