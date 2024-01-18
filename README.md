# Process Writeup

## Name: Josiah Benitez
## Course: SEP12
## Period: 7
## Concept: Unit 6

### Overview

Unit 6 is all about arrays and they are coded and used very similarly to javascript. On the Unit 6 exam I got some questions wrong and here I document one of them as well as overarching problems I had throughout the whole Unit.
## First Challenge
### Method Madness

On the Unit 6 exam I got question 2 wrong and here is the code to that question

```java
public static int mystery(double[] a,double x)
{
  int s = 0;
  for (int i = 0; i < a.length; i++)
  {
    if (a[i] != x)
    {
      s = s + a[i] ;
    }
  }
  return s;
}

```
 
The question is simply asking what does this code do and my answer to that was "Returns the sum of the values in the array". What I messed up on and what eventually cost me the question was the fact that it does ask for a sum but only if none of the values in the array are equal to X. The code `if(a[i] != x)` assures that it wont ask for a sum if x is equal to a value in the array and I missed this very important piece of code. This type of mistake makes up a sizeable percentage of my questions on this test so this will represent those. 


## Second Challenge
### IndexOutofBounds error

I ended up getting this error on a lot of the coding activities due to me writing code that would have the index be negative or have the index exceed the array length. For example:

```java
int[] numbers = {1, 2, 3, 4, 5};
// Accessing an element outside the array bounds
int value = numbers[5]; // This will result in an ArrayIndexOutOfBoundsException
```

This error occurs when trying to access an array element outside of the valid range. This can happen a lot when you miscount your elements in the array forgetting that the first element is always counted as the index of 0. A simple solution to this would be the following:

```java
int index = 2;
if (index >= 0 && index < numbers.length) {
    int value = numbers[index];
    System.out.println("Value at index " + index + ": " + value);
} else {
    System.out.println("Index out of bounds");
}
```

This checks if the index is withing the valid range first before trying to access it, therefore effectively solving this issue.

## Third Challenge
### Modyfing Arrays within a loop





### Takeaways

* Always make sure you are trying to access an element within a valid range so you don't run into an errorw
* Be careful when using a for each loop because modifying the array can lead to problems due to the iterator running internally.
* Put more time towards questions that require more reading of code so you are less likely to skim over important code.
* 
