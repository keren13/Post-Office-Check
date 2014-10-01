Post-Office-Check
=================

When mailing packages first class, the U.S. post office service has certain restrictions. Shipping does not occur in this scenario if the box has a girth and length greater than 100 inches  or if the weight is over 70 pounds. These calculations are determined and declared in the following program.

/** import java.util.Scanner;
    import java.io.*;   
    */
import java.util.Scanner;
import java.io.*;
    
public class MailCheck

{
public static void main(String args[])

   { 

       
 System.out.println("Inut a dimension: ");
 Scanner in = new Scanner(System.in);
 int dimensionThree = in.nextInt();
 
 System.out.println("Input weight: ");
 int weight = in.nextInt();
 
 System.out.println("Input a dimension: ");
 int dimensionOne = in.nextInt();
 
 System.out.println("Input a dimension: ");
 int dimensionTwo = in.nextInt();
 

 
 if(dimensionOne < dimensionTwo && dimensionThree < dimensionTwo){
     int length = dimensionTwo;
    }
    
    if(dimensionOne > dimensionTwo && dimensionOne > dimensionThree){
       int length = dimensionOne;
    }
    
    if(dimensionThree > dimensionOne && dimensionThree > dimensionTwo){
        int length = dimensionThree;
    }
    
    int girth = (dimensionThree * dimensionTwo * dimensionOne);
    //int weight;
    int length;
    //int girth;
    
    if(weight > 70 &&  girth > 100){
    System.out.println("Package is too large and too heavy.");
   } 
   
   if(weight > 70 &&  girth < 100){
       System.out.println("Package is too heavy.");
    }
    
    if(girth > 100 && weight < 70){
        System.out.println("Package is too heavy.");
    }
    
    if(girth < 101 && weight <= 70){
        System.out.println("Package is acceptable");
    }

 
}
}
