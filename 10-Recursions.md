## Name: Wilson Huang
## Course: APCSA
## Period: 7
## Concept: Unit 10

### Introduction
In APCSA we are learning Unit 10 (Recursions) which is our last unit in APCSA. This unit was confusing since recursions can be hard to understand. I did okay on the quiz but I didn't do too well on the unit 10 examn. In this writeup I will take you through some of the challenges I had and the questions I for wrong in the exam. 

### Challenge #1
One challenge I had when learning unit 10 is figuring out how recursions work and the sequence it has. To figure this out I went to phython tutor where it shows each step it goes through to better understand how it works. Recursions is basically a function that calls itself and does not stop until it reaches the base. 
``` java
public static void printNumber(int n)
{
  if (n >= 10)
  {
    printNumber(n / 10);
  }
  System.out.println(n % 10);
}
```
When n = 1497, it is greater than 10 so we divide it by 10. 149 is greater than 10 so we divide by 10 again to then get 14. This is also greater than 10 we divide by 10 to get 1. I then gets the remaindars of the numbers that were divided by 10. I then prints this:
```
1
4
9
7
```
### Challenge #2
Another challenge I had when learning unit 10 is understanding merge sort and binary search. These lessons were confusing to understand what it does. To understand this I went to youtube to watch videos about it. I watched this video about [merge sort](https://www.youtube.com/watch?v=3j0SWDX4AtU) and this video about [binary search](https://www.youtube.com/watch?v=xrMppTpoqdw). I learned that merege sort is when you divide a array into smaller pieces and sorting each seperated array and then combining it. Binary search is when you keep diving a sorted array to find what you are finding. 

### Challenge #3
The last challenge I had was the exam. I did not do too well in this exam. So in this challenge I will take you through 3 questions I had a hard time answering. 

#### Challenge #3.1

#### Challenge #3.2

#### Challenge #3.3

### Takeaways
* Search on youtube if you do not understand a certain topic because there is a lot of online resources that can help you
* Go over the questions you got wrong in the exam because that is how you learn
* 

