1.Java Program: Are you above 18 years old? 
package day_2;
 import java.util.Scanner;
 public class EligibleAge {
 public static void main(String[] args) { 
  Scanner input = new Scanner(System.in);  
  System.out.print("Please enter your age: "); 
  int age = input.nextInt();  
  if (age > 18) {  
              System.out.println("You are eligible to vote.");  
          } else { 
              System.out.println("You are not eligible to vote 
yet."); 
              } 
  input.close();  
     } 
  
 } 
Output:  
Please enter your age: 22
 You are eligible to vote.
 2.Java Program: Print Multiplication Table Using for Loop 
package day_2;
 import java.util.Scanner; 
public class MultiplicationTable { 
 public static void main(String[] args) { 
    Scanner input = new Scanner(System.in); 
    System.out.print("Enter a number to print its multiplication table: "); 
    int number = input.nextInt(); 
    System.out.println("Multiplication table for " + number + ":"); 
    for (int i = 1; i <= 10; i++) { 
              int result = number * i;  
              System.out.println(number + " x " + i + " = " + result);  
          } 
    input.close(); 
 
 } 
 
}
 Output:  
Enter a number to print its multiplication table: 5
 Multiplication table for 5:
 5 x 1 = 5
 5 x 2 = 10
 5 x 3 = 15
 5 x 4 = 20
 5 x 5 = 25
 5 x 6 = 30
 5 x 7 = 35
 5 x 8 = 40
 5 x 9 = 45
 5 x 10 = 50
 3.Java Program: Character, String, and Boolean Input 
Example 
package day_2;
 import java.util.Scanner; 
public class UserInputSummary { 
 public static void main(String[] args) { 
  // TODO Auto-generated method stub 
          Scanner scanner = new Scanner(System.in); 
          System.out.print("Enter a single character: "); 
          char character = scanner.next().charAt(0); 
          System.out.print("Enter your name: "); 
          String name = scanner.next(); 
          System.out.print("Do you like programming? (true/false): "); 
          boolean likesProgramming = scanner.nextBoolean(); 
          System.out.println("\n--- User Input Summary ---"); 
          System.out.println("Character entered: " + character); 
          System.out.println("Name entered: " + name); 
          System.out.println("Likes programming: " + likesProgramming); 
          if (likesProgramming) { 
              System.out.println("Great! Keep coding, " + name + "!"); 
          } else { 
              System.out.println("No worries! Programming isn't for everyone."); 
          } 
          scanner.close(); 
      } 
} 
Output: 
Enter a single character: s
 Enter your name: sudha
 Do you like programming? (true/false): true--- User Input Summary --
Character entered: s
 Name entered: sudha
 Likes programming: true
 Great! Keep coding, sudha!
 4.Simple Banking Operations using switch Case 
package day_2;
 import java.util.Scanner;
 public class SimpleBanking { 
 public static void main(String[] args) { 
  Scanner scanner = new Scanner(System.in); 
        int balance = 0; 
        int choice; 
        System.out.println("Welcome to ABC Bank"); 
        while (true) { 
            System.out.println("\n1. Check Balance"); 
            System.out.println("2. Deposit Money"); 
            System.out.println("3. Withdraw Money"); 
            System.out.println("4. Exit"); 
            System.out.print("Enter your choice: "); 
            choice = scanner.nextInt(); 
            switch (choice) { 
                case 1: 
                    System.out.println("Your current balance is: " + balance); 
                    break; 
                case 2: 
₹
                    System.out.print("Enter amount to deposit: "); 
                    int deposit = scanner.nextInt(); 
                    if (deposit > 0) { 
                        balance += deposit; 
                        System.out.println("Deposit successful!"); 
                    } else { 
                        System.out.println("Invalid deposit amount."); 
                    } 
                    break; 
                case 3: 
                    System.out.print("Enter amount to withdraw: "); 
                    int withdraw = scanner.nextInt(); 
                    if (withdraw > 0 && withdraw <= balance) { 
                        balance -= withdraw; 
                        System.out.println("Withdrawal successful!"); 
                    } else if (withdraw > balance) { 
                        System.out.println("Insufficient balance."); 
                    } else { 
                        System.out.println("Invalid withdrawal amount."); 
                    } 
                    break; 
                case 4: 
                    System.out.println("Thank you for using ABC Bank!"); 
                    scanner.close(); 
                    return; 
                default: 
                    System.out.println("Invalid choice. Please try again."); 
                    } 
        } 
 } 
} 
Output: 
Welcome to ABC Bank
 1. Check Balance
 2. Deposit Money
 3. Withdraw Money
 4. Exit
 Enter your choice: 1
 Your current balance is: 0
 1. Check Balance
 2. Deposit Money
 3. Withdraw Money
 4. Exit
 Enter your choice: 2
 ₹
 Enter amount to deposit: 200
 Deposit successful!
 1. Check Balance
 2. Deposit Money
 3. Withdraw Money
 4. Exit
 Enter your choice: 2000
 Invalid choice! Please try again.
 1. Check Balance
 2. Deposit Money
 3. Withdraw Money
 4. Exit
 Enter your choice: 3
 Enter amount to withdraw: 200
 Withdrawal successful!
 1. Check Balance
 2. Deposit Money
 3. Withdraw Money
 4. Exit
 Enter your choice: 3
 Enter amount to withdraw: 5000
 Insufficient balance!
 1. Check Balance
 2. Deposit Money
 3. Withdraw Money
 4. Exit
Enter your choice: 
5.Task: Create a program that accepts age, height, and weight of a person and 
prints them with appropriate data types. 
package day_2;
 import java.util.Scanner; 
public class PrimitiveData {
 public static void main(String[] args) { 
Scanner scanner = new Scanner(System.in); 
System.out.print("Enter Age: "); 
int age = scanner.nextInt(); 
System.out.print("Enter Height: "); 
float height = scanner.nextFloat(); 
System.out.print("Enter Weight: "); 
double weight = scanner.nextDouble(); 
System.out.println("\nAge: " + age); 
System.out.println("Height: " + height); 
System.out.println("Weight: " + weight); 
scanner.close(); 
} 
} 
Output: 
Enter Age: 22
 Enter Height: 4.5
 Enter Weight: 45
 Age: 22
 Height: 4.5
 Weight: 45.0
 6.Task: Declare and initialize different types of variables to store a student’s 
information: ID, name, marks, and grade.Print them. 
package day_2;
 public class StudentInfoVaria {
 public static void main(String[] args) { 
int id = 101; 
String name = "Sudha"; 
double marks = 98.8; 
char grade = 'A'; 
System.out.println("Student ID: " + id); 
System.out.println("Name: " + name); 
System.out.println("Marks: " + marks); 
System.out.println("Grade: " + grade); 
} 
} 
Output: 
Student ID: 101
 Name: Sudha
 Marks: 98.8
 Grade: A
 7.Task: Accept two numbers and perform arithmetic, relational, and logical 
operations on them 
package day_2;
 import java.util.Scanner; 
public class Operators {
public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter number1: "); 
int num1 = sc.nextInt(); 
System.out.print("Enter number2: "); 
int num2 = sc.nextInt(); 
System.out.println("Addition: " + (num1 + num2)); 
System.out.println("Greater number: " + (num1 > num2 ? num1 : num2)); 
System.out.println("Are both positive? " + (num1 > 0 && num2 > 0)); 
sc.close(); 
} 
} 
Output: 
Enter number1: 20
 Enter number2: 10
 Addition: 30
 Greater number: 20
 Are both positive? true
 8.Task: Create a greeting message using first name and last name entered by the 
user. 
package day_2;
 import java.util.Scanner; 
public class Message {
 public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter First Name: "); 
String firstName = sc.nextLine(); 
System.out.print("Enter Last Name: "); 
String lastName = sc.nextLine(); 
String welcomeMessage = "Hello " + firstName + " " + lastName + "!"; 
System.out.println(welcomeMessage); 
sc.close(); 
} 
} 
Output: 
Enter First Name: Raga
Enter Last Name: Sudha
 Hello Raga Sudha!
 9.Task: Accept a sentence and reverse it using StringBuilder 
package day_2;
 import java.util.Scanner; 
public class StringBuilderExample {
 public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter a sentence: "); 
String input = sc.nextLine(); 
StringBuilder sb = new StringBuilder(input); 
System.out.println("Reversed: " + sb.reverse()); 
sc.close(); 
} 
} 
Output: 
Enter a sentence: Hello Namaskaram
 Reversed: maraksamaN olleH
10.Task: Count how many times a specific character appears in a string. 
package day_2;
 import java.util.Scanner; 
public class CharacterCount {
 public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter a string: "); 
String str = sc.next(); 
System.out.print("Enter character to count: "); 
char ch = sc.next().charAt(0); 
long count = str.chars().filter(c -> c == ch).count(); 
System.out.println("Character '" + ch + "' appears " + count + " times."); 
sc.close(); 
} 
} 
Output: 
Enter a string: sudha
 Enter character to count: s
 Character 's' appears 1 times.
 11.Task: Display the current date and format it as DD-MMYYYY. 
package day_2;
 import java.text.SimpleDateFormat; 
import java.util.Date; 
public class CurrentDate { 
public static void main(String[] args) { 
Date date = new Date(); 
SimpleDateFormat sdf = new SimpleDateFormat("dd-MM-yyyy"); 
System.out.println("Current Date: " + sdf.format(date)); 
} 
} 
Output: 
Current Date: 24-07-2025 
12.Task: Based on a number entered, print whether it's positive, negative, or 
zero. 
package day_2;
 import java.util.Scanner; 
public class NumberCheck { 
public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter a number: "); 
int number = sc.nextInt(); 
if (number > 0) System.out.println("The number is positive."); 
else if (number < 0) System.out.println("The number is negative."); 
else System.out.println("The number is zero."); 
sc.close(); 
} 
} 
Output: 
Enter a number: 69
 The number is positive.
 13.Task: Accept marks and display the grade using if-else. 
package day_2;
 import java.util.Scanner; 
public class Grade {
 public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter marks: "); 
int marks = sc.nextInt(); 
if (marks >= 90) System.out.println("Grade: A"); 
else if (marks >= 75) System.out.println("Grade: B"); 
else if (marks >= 60) System.out.println("Grade: C"); 
else System.out.println("Grade: D"); 
sc.close(); 
} 
} 
Output: 
Enter marks: 69
 Grade: C
 14.Task: Build a simple calculator using switch to perform operations (+, -, 
*, /). 
package day_2;
 import java.util.Scanner; 
public class Arithmetic {
 public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter number1: "); 
double num1 = sc.nextDouble(); 
System.out.print("Enter number2: "); 
double num2 = sc.nextDouble(); 
System.out.print("Enter operation (+, -, *, /): "); 
char op = sc.next().charAt(0); 
switch (op) { 
case '+': System.out.println("Result: " + (num1 + num2)); break; 
case '-': System.out.println("Result: " + (num1 - num2)); break; 
case '*': System.out.println("Result: " + (num1 * num2)); break; 
case '/': System.out.println("Result: " + (num2 != 0 ? (num1 / num2) : 
"Cannot divide by zero")); break; 
default: System.out.println("Invalid operation"); 
} 
sc.close(); 
} 
} 
Output: 
Enter number1: 20
 Enter number2: 10
 Enter operation (+, -, *, /): +
 Result: 30.0
 15.Task: Print the first N even numbers using a loop 
package day_2;
 import java.util.Scanner; 
public class EvenLoop {
 public static void main(String[] args) { 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter N: "); 
int n = sc.nextInt(); 
for (int i = 0; i < n * 2; i += 2) { 
System.out.print(i + " "); 
} 
sc.close(); 
} 
} 
Output: 
Enter N: 10
 0 2 4 6 8 10 12 14 16 18 
16.Task: Accept 5 numbers, store them in an array, and display their average. 
package day_2;
 import java.util.Scanner; 
public class Array_Ave {
 
 public static void main(String[] args) { 
  Scanner sc = new Scanner(System.in); 
        int[] arr = new int[5]; 
        int sum = 0; 
        System.out.println("Enter 5 numbers:"); 
        for (int i = 0; i < 5; i++) { 
            arr[i] = sc.nextInt(); 
            sum += arr[i]; 
        } 
        System.out.println("Average: " + (sum / 5.0)); 
        sc.close(); 
 
 } 
 
} 
Output: 
Enter 5 numbers:
 2
 4
 5
 6
 7
 Average: 4.8
 17.Task: Create an enum for days of the week. Print a message depending on the 
day.
 
package day_2;
 enum WeekDay {
    MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY,
    SATURDAY, SUNDAY
 }
 public class EnumDay {
    public static void main(String[] args) {
        WeekDay today = WeekDay.SUNDAY;
        switch (today) {
            case MONDAY:
                System.out.println("New week, new goals!");
                break;
            case FRIDAY:
                System.out.println("Weekend is near!");
                break;
            case SUNDAY:
                System.out.println("Time to relax and recharge.");
                break;
            default:
                System.out.println("It's a regular weekday.");
        }
    }
 }
 Output: 
Time to relax and recharge.
