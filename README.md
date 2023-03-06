# java-Write a program to take "n" String inputs from user and store them in array (where "n" is no. of String objects specified by user at run-time). Sort the array in ascending order and display the array. If "n" entered by user is less than 2, then display message "Invalid".

Input Format

Your program should take the input of "n" string objects.

Constraints

No. of string objects entered by the user should be greater than 1.

Output Format

Your program should display the array of strings in sorted ascending order.

Sample Input 0

4
India
America
Australia
France
Sample Output 0

America
Australia
France
India
Contest ends in 17 hours
Submissions: 30
Max Score: 5
Difficulty: Medium
Rate This Challenge:

    
More
 
1
import java.util.Arrays;
2
import java.util.Scanner;
3
​
4
public class SortStrings {
5
​
6
    public static void main(String[] args) {
7
        
8
        // create a Scanner object to take input from user
9
        Scanner sc = new Scanner(System.in);
10
        
11
        // take input of "n" string objects
12
       // System.out.print(" ");
13
        int n = sc.nextInt();
14
        
15
        // check if n is less than 2
16
        if (n < 2) {
17
            System.out.println("Invalid");
18
            return;
19
        }
20
        
21
        // create an array to store the strings
22
        String[] arr = new String[n];
23
        
24
        // take input of the strings from the user and store them in the array
25
        //System.out.println("");
26
        for (int i = 0; i < n; i++) {
27
            arr[i] = sc.next();
28
        }
29
        
30
        // sort the array in ascending order
31
        Arrays.sort(arr);
32
        
33
        // display the sorted array
34
       // System.out.println("");
35
        for (String str : arr) {
36
            System.out.println(str);
37
        }
38
    }
39

40
}
