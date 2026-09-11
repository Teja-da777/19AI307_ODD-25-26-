# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION: 
Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)

## AIM: 
To write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Uses System.in to accept input from the keyboard.
4. Uses InputStreamReader to convert byte streams into character streams.
5. Uses BufferedReader for efficient character input.
6. Demonstrates how one stream can be wrapped inside another stream.
7. Uses readLine() to read complete lines of user input.
8. Demonstrates proper stream closing after completing the input operation.


## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: THEJESWARAN M
RegisterNumber: 212223240168
*/
```

## SOURCE CODE:
```
import java.io.BufferedReader;
import java.io.InputStreamReader;

public class Main {
    public static void main(String[] args){
        
        try {
            
            BufferedReader br = new BufferedReader(
                    new InputStreamReader(System.in));

            String name = br.readLine();
            int age = Integer.parseInt(br.readLine());

            System.out.println("--- User Details ---");
            System.out.println("Name: " + name);
            System.out.println("Age: " + age);

        } 
        
        catch (Exception e) {
            System.out.println("Error");
        }
        
    }
    
}
```


## OUTPUT:
<img width="978" height="422" alt="Screenshot 2026-09-11 211128" src="https://github.com/user-attachments/assets/92b9736b-aa5e-4efd-9eb1-e15e862d2a21" />


## RESULT:
Thus the program successfully BufferedReader on top of InputStreamReader on top of System.in.
