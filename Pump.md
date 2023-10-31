# javaNotebook
final variable in java

final int number = 12
number =14 // it will throw error as we cannot reassign value to final one's


assigning same value to multiple variables
int x, y, z;
x = y = z = 50;
System.out.println(x + y + z);

OR 

int x = 5, y= 3 , z=4;
System.out.println(x+y+z);
>> output will be : 12


primitive data type starts with small letter while non-premitive starts with capital letter like (int and String)

STRING add ons 
txt.length()
------------------------
System.out.println(txt.toUpperCase());   // Outputs "HELLO WORLD"
System.out.println(txt.toLowerCase());   // Outputs "hello world"
------------------------
String txt = "Please locate where 'locate' occurs!";
System.out.println(txt.indexOf("locate")); // Outputs 7
------------------------
String firstName = "John ";
String lastName = "Doe";
System.out.println(firstName.concat(lastName));
>> John Doe
~~~~~~~~~~Java uses the + operator for both addition and concatenation.
~~~~~~~~~~Numbers are added. Strings are concatenated.
~~~~~~~~~~If you add a number and a string, the result will be a string concatenation:
String x = "10";
int y = 20;
String z = x + y;  // z will be 1020 (a String)
--------------------------------------
Special character in java 
to use ' " or \ in java string you can use a backslash before ex
\' , \" , \\

others
\b - tick
\r, \n - new line
\t - tab spacing
---------MATH-----------
Math.max(x,y,z)
Math.min(x,y,z)
Math.sqrt(64)
Math.abs(-12.4) // positive absolute value i.e 12.4
Math.random() // value between 0.0 to 1.0
int randomNum = (int)(Math.random() * 101);  // 0 to 100
-----------ternary operator in java-----------
var jash = (condition) ? expressionTrue : expressionFalse;
----------SWITCH EXAMPLE--------------
int num = 2;
switch(num) {
  case 1:
    System.out.println("Monday");
    break;
  case 2:
    System.out.println("Tuesday");
    break;
  default:
    System.out.println("OtherDay");
}
-----------FOR LOOP-----------
// Outer loop
for (int i = 1; i <= 2; i++) {
  System.out.println("Outer: " + i); // Executes 2 times
  
  // Inner loop
  for (int j = 1; j <= 3; j++) {
    System.out.println(" Inner: " + j); // Executes 6 times (2 * 3)
  }
} 
------------For Each loop----------
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
for (String i : cars) {
  System.out.println(i);
}
--------BREAK AND CONTINUE--------
break - stop the loop
continue - skip the one specific condition
----------ARRAY IN JAVA----------
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
-----------Multi dimensional array--------
int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
System.out.println(myNumbers[1][2]); // Outputs 7
public class Main {
  public static void main(String[] args) {
    int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
    for (int i = 0; i < myNumbers.length; ++i) {
      for(int j = 0; j < myNumbers[i].length; ++j) {
        System.out.println(myNumbers[i][j]);
      }
    }
  }
}
