# D2a6

1) Write a program to accepts two numbers from stdin and find all the odd as well as even
numbers present in between them.

Solution:


import java.util.ArrayList; import java.util.Scanner;

public class acad {
public static void main(String[] args){
Scanner sc=new Scanner(System.in); int a=sc.nextInt(); //accepting value of first integer from user 
int b=sc.nextInt(); //accepting value of second integer from user 
ArrayList odd=new ArrayList();
ArrayList even=new ArrayList(); 
for(int i=a;i<=b;i++){
if(i%2==0) even.add(i); //Storing even numbers in arraylist else odd.add(i);//Storing odd numbers in arraylist
}
System.out.println("Odd numbers are:\n");
    for(int i:odd)
        System.out.print(i+" ");
 System.out.println("\nEven numbers are:\n");
    for(int i:even)
        System.out.print(i+" ");
}
}

2) Joe is scared to go to school. When her dad asked the reason, joe said she is unable to complete the task given by her teacher. The task was to find the “first 10 multiples” of the number entered from stdin.

Solution:

import java.util.Scanner;

public class acad {
public static void main(String[] args){
Scanner sc=new Scanner(System.in); 
int n=sc.nextInt(); //accepting the number
System.out.println("Input: "+n); 
System.out.println("O/p:"); 
for(int i=1;i<=10;i++){ 
System.out.println(n+" * "+i+" = "+(n*i)); //displaying table of given number
}
}
}


3) Write a program consisting method sum() and demonstrate the concept of method overloading using this method.

Solution:

import java.util.Scanner;

public class acad { 
public static void main(String[] args){ 
Scanner sc=new Scanner(System.in); int a=sc.nextInt();   //Accepting 3 numbers from the user
int b=sc.nextInt();
int d=sc.nextInt(); 
sum(a,b); 
sum(a,b,d); }        // method overloading
public static void sum(int a,int b){
System.out.println("Sum of first 2 numbers is:"+(a+b));
} 
public static void sum(int a,int b,int d){
System.out.println("Sum of all 3 numbers is:"+(a+b+d)); } 
}
