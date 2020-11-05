Coding Exercise 1: Speed Converter
```java
public class SpeedConverter {
    public static long toMilesPerHour(double kilometersPerHour){
        if(kilometersPerHour >= 0){
            return Math.round(kilometersPerHour / 1.609);
        }
        return -1;
    }
    public static void printConversion(double kilometersPerHour){
        if(kilometersPerHour<0){
            System.out.println("Invalid Value");
        }
        else{
        System.out.println(kilometersPerHour+" km/h = "+toMilesPerHour(kilometersPerHour)+" mi/h");}
    }
}
```
Coding Exercise 2: MegaBytes Converter
```java
public class MegaBytesConverter {
    public static void printMegaBytesAndKiloBytes(int kiloBytes){
        if(kiloBytes < 0)
            System.out.println("Invalid Value");
        else
           System.out.println(kiloBytes+" KB = "+(kiloBytes/1024)+" MB and "+(kiloBytes%1024)+" KB");
    }
}
```
Coding Exercise 3: Barking Dog
```java
public class BarkingDog {
  public static boolean shouldWakeUp(boolean baking, int hourOfDay){
        if(baking && (hourOfDay>=0 && hourOfDay < 8) || (hourOfDay > 22 && hourOfDay < 24)){
           return true;
        }
        return false;
    }
}
```
Coding Exercise 4: Leap Year Calculator
```java
public class LeapYear {
 public static boolean isLeapYear(int year){
       if(year % 4 == 0 && ( year >= 1 && year<=9999 )){
           if(year % 100 == 0){
               if(year % 400 == 0){
                   return true;
               }
           }
           else {
               return true;
           }
       }
        return false;
    }
}
```
Coding Exercise 5: DecimalComparator
```java
public class DecimalComparator{
    public static boolean areEqualByThreeDecimalPlaces(double num1, double num2){
        long convertedA = (int)(num1 * 1000);
        long convertedB = (int)(num2 * 1000);
        return convertedA == convertedB;
    }
 
}
```
Coding Exercise 6: Equal Sum Checker
```java
public class EqualSumChecker {
    public static boolean hasEqualSum(int num1, int num2, int num3){

        return (num1+num2) == num3;
    }
}
```
Coding Exercise 7: Teen Number Checker
```java
public class TeenNumberChecker {
 public static boolean hasTeen(int num1, int num2, int num3){
         if (isTeen(num1) || isTeen(num2) || isTeen(num3)) return true;
         else return false;
    }
public static boolean isTeen(int age){
        if(age>=13 && age<=19) return true;
        else return false;
    }
}
```
Coding Exercise 8: Area Calculator
```java
public class AreaCalculator {
      public static double area(double radius){
        if(radius>=0){
           return Math.PI*radius*radius;
        }
        return -1.0;
    }

    public static double area(double x, double y){
        if(x>=0 && y>=0){
            return x*y;
        }
        else return -1;
    }
}
```
Coding Exercise 9: Minutes To Years and Days
```java
public class MinutesToYearsDaysCalculator {
    public static void printYearsAndDays(long minutes){
        if(minutes < 0){
           System.out.println("Invalid Value");
        }
        else {
            System.out.println(minutes+" min = "+minutes/525600L+" y and "+(minutes % 525600L)/1440L+" d");
        }
    }
}
```
Coding Exercise 10: Equality Printer
```java
public class IntEqualityPrinter {
    public static void printEqual(int num1, int num2 ,int num3){
        if(num1 < 0 || num2 < 0 || num3 < 0) System.out.println("Invalid Value");
        else if( num1==num2 && num2==num3 ) System.out.println("All numbers are equal");
        else if( num1!=num2 && num2!=num3 && num3!=num1 ) System.out.println("All numbers are different");
        else System.out.println("Neither all are equal or different");
    }
}
```
Coding Exercise 11: Playing Cat
```java
public class PlayingCat {
    public static boolean isCatPlaying(boolean summer,int temperature){
      if(summer && temperature>=25 && temperature<=45) return true;
      else if(!summer && temperature>=25 && temperature<=35) return true;
      else return false;
    }
}
```