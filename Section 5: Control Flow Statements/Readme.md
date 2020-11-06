Coding Exercise 12: Number In Word
```java
public class NumberInWord {
    public static void printNumberInWord(int val){
      switch (val) {
          case 0:
              System.out.println("ZERO"); break;
          case 1:
              System.out.println("ONE"); break;
          case 2:
              System.out.println("TWO"); break;
          case 3:
              System.out.println("THREE"); break;
          case 4:
              System.out.println("FOUR"); break;
          case 5:
              System.out.println("FIVE"); break;
          case 6:
              System.out.println("SIX"); break;
          case 7:
              System.out.println("SEVEN"); break;
          case 8:
              System.out.println("EIGHT"); break;
          case 9:
              System.out.println("NINE"); break;
          default:
              System.out.println("OTHER");
      }
    }
}
```
Coding Exercise 13: Number Of Days In Month
```java
public class NumberOfDaysInMonth {
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

    public static int getDaysInMonth(int month, int year){
        if( month<1 || month>12 || year<1 || year>9999){
            return -1;
        }
        int[] leap_yr = {31,29,31,30,31,30,31,31,30,31,30,31};
        int[] non_leap_yr = {31,28,31,30,31,30,31,31,30,31,30,31};
        if(isLeapYear(year)){
            return leap_yr[month-1];
        }
        else {
            return non_leap_yr[month-1];
        }
    }
}
```
Coding Exercise 14: Sum Odd
```java
public class SumOddRange {
 public static boolean isOdd(int number){
        if (number<0) return false;
        if (number%2!=0) return true;
        else return false;
    }
    public static int sumOdd(int start, int end){
        if(end < start || end<0 || start<0){
            return -1;
        }
        else {
            int count = 0;
            for(int i = start ; i <= end ; i++){
                if (isOdd(i)) count+=i;
            }
            return count;
        }
}
}
```
Coding Exercise 15: Number Palindrome
```java
public class NumberPalindrome {
 public static boolean isPalindrome(int number){
        int temp = number;
        int rev = 0;
        while(temp!=0){
            rev = rev*10 + temp%10;
            temp /= 10;
        }
        return rev == number;
    }
}
```
Coding Exercise 16: First And Last Digit Sum
```java
public class FirstLastDigitSum {
     public static int sumFirstAndLastDigit(int number){
        if(number<0) return -1;
        else if(number == 0) return 0;
        else return number%10 + (int)(number / (int)(Math.pow(10, (int)(Math.log10(number)))));
    }
}
```
Coding Exercise 17: Even Digit Sum
```java
public class EvenDigitSum {
    public static int getEvenDigitSum(int number){
        if(number<0) return -1;
        else {
           int sum = 0;
           while(number!=0){
              int temp = number%10;
              if(temp%2==0){
                  sum +=temp;
              }
              number /=10;
           }
           return sum;
        }
    }   
}
```
Coding Exercise 18: Shared Digit
```java
public class SharedDigit {
    public static boolean hasSharedDigit(int num_1,int num_2){
      if(num_1<10 || num_1>99 || num_2<10 || num_2>99) return false;
      if ((num_1%10 == num_2/10) || (num_1/10 == num_2%10) || (num_1%10 == num_2%10) || (num_1/10 == num_2/10)) return true;
      return false;
    }
}
```
Coding Exercise 19: Last Digit Checker
```java
public class LastDigitChecker {
    public static boolean hasSameLastDigit(int num_1,int num_2, int num_3){
        if(num_1<10 || num_1>1000 || num_2<10 || num_2>1000 || num_3<10 || num_3>1000 ) return false;
        if ((num_1%10 == num_2%10) || (num_2%10 == num_3%10) || (num_1%10 == num_3%10)) return true;
      return false;
    }
    public static boolean isValid(int num) {
        if(num<10 || num>1000) return false;
        return true;
    }
}
```
Coding Exercise 20: Greatest Common Divisor
```java
public class GreatestCommonDivisor {
   public static int getGreatestCommonDivisor(int first , int second) {
        if( first<10 || second<10 ) return -1;
        else {
            while (first != second) {
                if(first > second)
                    first = first - second;
                else
                    second = second - first;
            }
        }
        return second;
    }
}
```
Coding Exercise 21: All Factors
```java
public class FactorPrinter {
public static void printFactors(int number) {
       if(number<1){
           System.out.print("Invalid Value");
       }
       else {
           for (int i = 1 ; i <= number ; i++){
               if(number%i == 0)
                   System.out.print(i+" ");
           }
       }
    }
}
```
Coding Exercise 22: Perfect Number
```java
public class PerfectNumber {
        public static boolean isPerfectNumber(int number) {
        if (number < 1) {
            return false;
        } else {
            int sum = 0;
            for (int i = 1; i < number; i++) {
                if (number % i == 0)
                    sum += i;
            }
            if (sum == number) return true;
            else return false;
        }
    }
    
}
```
Coding Exercise 23: Number To Words
```java

```
Coding Exercise 24: Flour Pack Problem
```java

```
Coding Exercise 25: Largest Prime
```java

```
Coding Exercise 26: Diagonal Star
```java

```
Coding Exercise 27: Input Calculator
```java

```
Coding Exercise 28: Paint Job
```java

```