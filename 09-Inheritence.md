## Name: Wilson Huang
## Course: APCSA
## Period: 7
## Concept: Unit 9

### Introduction
In APCSA (AP Computer Science A) we are curretly learning about inheritence (unit 9). This unit has been confusing and challenging for me since a lot of new concepts were introduced to me. I didn't do to well on the quiz and exam so throughout this write up I will take you through my challenges I had and some of the questions I got wrong on the tests. 

### Challenge #1
One challenge I had when learning inheritaence is learning what and how to use `super()`. I was confused on when to use it and hot it works. To understand this I watched youtube videos about this. For example I watched [this](https://www.youtube.com/watch?v=oKZnHNM9Ew4) video that helped me understand what `super()` is. Throughout this video I learned that `super()` can access constructors and methods in the parent class but not all like private methods.
``` java
public String toString(){
    return super.toString() + " with " + flavor;
}
```

### Challenge #2
Another challenge I faced when learning unit 9 is what a child class can or cannot inherit from the parent class but by reading this [page](https://www.codecademy.com/learn/learn-java/modules/learn-java-inheritance-and-polymorphism/cheatsheet) from codeacademy I learned that it can't inherit the private costructors. 
```java
private print() { \\cannot access this
    System.out.println("Hello");
}

```


### Challenge #3
In this challenge I will take you through some of the questions I got wrong on the unit test

#### Challenge #3.1 - 3.2
``` java
public class A
{
  public A()
  {
    System.out.print("one orange ");
  }
  
  public A(int z)
  {
    System.out.print("two oranges ");
  }

  public void doStuff()
  {
    System.out.print("six oranges ");
  }
}

public class B extends A
{
  public B()
  {
    super();
    System.out.print("three oranges ");
  }

  public B(int val)
  {
    super(val);
    System.out.print("four oranges ");
  }
}
```
##### Challenge 3.1
What is `A a = new B(5);`?
For this question I chose `four oranges` but it was wrong because I thought it would go directly to `public B(int val)` and print `four oranges`. I learned that if I create a new class of `b`, it goes to `int val` so the constructor prints two oranges and four oranges. 
##### Challenge 3.2
What is printed when the following line of code is executed? 
`b.doStuff();` 
For this question I chose `Nothing is printed, an error occurs` because I thought this because b does not have the method `dostuff` but I was wrong because it extends to A and prints out `six oranges`.



#### Challenge #3.3
```java
public class Conversation
{
 // default constructor automatically added to this class
  public void hello()
  {
    System.out.println("Hello");
  }
  public void greeting()
  {
    hello();
    System.out.println("Nice to meet you");
  }
}

public class PoliteConversation extends Conversation
{
 // default constructor automatically added to this class
  public void hello()
  {
    super.hello();
    System.out.println("What a pleasant surprise!");
  }
  public void greeting()
  {
    super.greeting();
    System.out.println("I hope you’re doing well");
  }
} 
```
What is printed as a result of the call conv.greeting()? For this question I chose Hello and Nice to meet you. However this is wrong because the methods for PoliteConversation are declared so the answer is Hello, What a pleasant surprise!, Nice to meet you, I hope you’re doing well

### Takeaways
* Look on the internet if you have any misconceptions
* Reciew questions you got wrong
