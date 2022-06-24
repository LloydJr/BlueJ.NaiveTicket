# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

First you need to FORK this repo into your account, then you need to CLONE that foreked repo, the one in your account. 
When you are finished with your code, be sure to ADD/COMMIT and PUSH your code to your repo.

Use the URL from your repo as the submission to the portal. 

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
    * You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket?
------0-----
### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
    * Do you notice anything strange about the machine’s behavior?
-----The machine is a little buggy and does not reduce the amount to zero after you print the ticket.-----
    * What happens if you insert too much money into the machine – do you receive any refund?
-----The machine did not give me my refund :(-----
    * What happens if you do not insert enough and then try to print a ticket?
-----What happen was when I inserted 3 cents, I was still able to print a ticket.-----
### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.

### Exercise 2.5
* Create another ticket machine for tickets of a different price.
    * Buy a ticket from that machine.
    * Does the printed ticket look different?
-----The printed ticket does look different.-----
### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part.
* -----The outter wrapper of a student would be "public class Student" and LabClass would be "public class LabClass".-----

### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class?
-----It does matter because the code would not be able to function if the "public" is not in front of class.-----
* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
    * Do you notice a change in the class diagram?
-----Yes! A syntax error would occur. The code would not function.-----
    * What error message do you get when you now press the compile button?
-----You would recieve <indentifier> expected.-----
    * Do you think this message clearly explains what is wrong?
------Yes and know but it does show that it is important that the order of how we write code can make a difference in an error.-----

### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class.
-----It is possible to leave out the word "public from the outter wrapper of the function.-----
### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
    * Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
    * Hint: There is only one constructor in the class.
-----Constructor == public class()-----
-----Field == private int <variable>-----
-----Methods == Ex: balance = balance + amount;-----
### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class?
-----The constructors initialize the object, also they have the same name such as "TicketMachine".-----
### Exercise 2.11
* What do you think is the type of each of the following fields?

```java
private int count;
-----Field-----
private Student representative;
-----Method-----
private Server host;
-----Constructor-----
```

### Exercise 2.12
* What are the names of the following fields?

```java
private boolean alive;
-----Method-----
private Person tutor;
-----Field-----
private Game game;
-----Constructor-----
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in?
-----In this case, the order does matter! Any other way would create a syntax error.-----
* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
    * Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are
possible?
    * Check by pressing the compile button to see if there is an error message.
    * Make sure that you reinstantiate the original version after your experiments!
-----It does matter which order the class is. The code is highlighted in green when it is functionable. It shows a syntax error when it is not functionable. So yes the ordering does matter.-----
### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration?
* Once again, experiment via the editor.
* The rule you will learn here is an important one, so be sure to remember it.
-----It is very necessary to have a semicolon at the end of a field declarartion. It tells the computer that that is the end of that line of code and if the semicolon is not present, a syntax error appears.-----

### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.
-----private int price;-----
### Exercise 2.16
* To what class does the following constructor belong?
```
public Student(String name)
```
-----The following constructor is an initializer, which shows the 'Student' class.-----
### Exercise 2.17
* How many parameters does the following constructor have and what are their types?
```
public Book(String title, double price)
```
-----There is one parameter, but two arguments.-----
### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be?
* Can you assume anything about the names of its fields?
-----It is hard to assume the types of fields might be because it can pretty much vary. But some that I have come up with would be books such as nonFiction, Fiction, and Documentaries.-----
READ upto and INCLUDING section 2.15 of this chapter.
