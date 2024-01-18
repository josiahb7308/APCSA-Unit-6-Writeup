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
The question is simply asking what does this code do and my answer to that was "Returns the sum of the values in the array". What I messed up on and what eventually cost me the question was the fact that it does ask for a sum but only if none of the values in the array are equal to X. The code `if(a[i] != x)` assures that it wont ask for a sum if x is equal to a value in the array and I missed this very important piece of code.


## Second Challenge
### Overthinking Obstacle

On question 15 I overthought this question so much that I changed the right answer I already selected into the wrong one. The answer I picked last which was wrong is the choice that says the procedure will work fine and nothing will be wrong, I was double checking my answers and I felt as if I picked the wrong answer even though I picked the right one so I changed it. The code in question is 
```java
/**
 * @param score - the student’s test score
 * @return the student’s letter grade
 */
public String closeEnough(int score)
  if (score >= 60) 
  {
    return “D”;
  } 
  else if (score >= 70) 
  {
    return “C”;
  } 
  else if (score >= 80) 
  {
    return “B”;
  } 
  else if (score >= 90) 
  {
    return “A”;
  } 
  else 
  {
    return “F”;
  }
```
The correct answer that I originally picked was that a score of 70 would cause the procedure to not work as expected because it would return a D instead of the C that it should actually return. 


## Third Challenge
### Compile-time 

For this challenge I got one of the two choices correct but I was stuck for the other part of the answer so I ended with the wrong answer. The code being looked at is the following:
```java
public class MyClass 
{
   public MyClass()
   {
     /* Implementation not shown */
   }
   public MyClass(int arg1) 
   {
     /* implementation not shown */
   }
   public MyClass(String arg1, int arg2) 
   {
     /* implementation not shown */
   }
}
```
I chose answer 3 which is correct and answer 2 which is wrong, here is why answer 2 is wrong. The constructor in 2 has a parameter which is of a String type, followed by a parameter which is an int. This is the same as a public constructor that is already included so this constructor cant be added to the class. 



### Takeaways

* When dealing with constructors pay close attention to the type of parameters they require and if there are any other constructors taking in the same parameters. This stems from my first challenge where I answered a question wrong because I didnt do this well.
* Look at what elements are public so you can adjust your parameters to not conflict with an already created constructor.
* I also had a mistake here that was made because of me overthinking my previous answer so I need to be more confident in my answers.
