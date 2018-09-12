# c212-Homework03import java.util.Scanner;

public class Grade {

    private double numberValue = 0;  
    private String value = "";

  public Grade(){
  
    Scanner in = new Scanner(System.in);
    System.out.print("Enter a number between 0 and 4: ");
    numberValue = in.nextDouble();
 }
 

  public String getNumericGrade() {

if(numberValue > 4)
   value = "Enter a smaller number"; 
if(numberValue <= 4 || numberValue >= 3.85)
   value = "A";
if(numberValue < 3.85 || numberValue >= 3.5)
   value = "A-";
if(numberValue < 3.5 || numberValue >= 3.15)
   value = "B+";
if(numberValue < 3.15 || numberValue >= 2.85)
   value = "B";
if(numberValue < 2.85 || numberValue >= 2.5)
   value = "B-";
if(numberValue < 2.5 || numberValue >= 2.15)
   value = "C+";
if(numberValue < 2.15 || numberValue >= 1.85)
   value = "C";
if(numberValue < 1.85 || numberValue >= 1.5)
   value = "C-";
if(numberValue < 1.5 || numberValue >= 1.15)
   value = "D+";
if(numberValue < 1.15 || numberValue >= 0.85)
   value = "D";
if(numberValue < 0.85 || numberValue >= 0.35)
   value = "D-";
if(numberValue < 0.35 || numberValue >= 0)
   value = "F"; 
if(numberValue < 0)
   value = "Enter a larger value";
  
return value;  

}
}
