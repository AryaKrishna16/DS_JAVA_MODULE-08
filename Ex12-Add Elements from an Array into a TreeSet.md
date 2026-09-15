# Ex12 Add Elements from an Array into a TreeSet
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
Create an array containing a few integer elements.
Create a TreeSet to store elements in sorted order.
Use a loop to add each element of the array into the TreeSet.
Display the elements of the TreeSet.
Stop the Program.   

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: E ARYA KRISHNA 
RegisterNumber: 212225240014 
*/
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        List<Integer> list = new ArrayList<>();
        for(int x : arr){
            list.add(x);
        }
        
        TreeSet<Integer> treeSet = new TreeSet<>(list);
        return treeSet;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}
```

## Output:
<img width="776" height="541" alt="image" src="https://github.com/user-attachments/assets/d8ff50fa-099e-45cf-b2a7-1ee8bcd2556e" />



## Result:
The program successfully adds elements from an array into a TreeSet.
