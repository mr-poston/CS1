# **👾 Chapter 1 Boss Battles: Hacking the Shapes**

*So, you finished the Core Labs early? It's time to look under the hood.*

Right now, you are using the BlueJ interface to create objects. But what if you want a shape to do something it wasn't programmed to do?

**Your Mission:** Open the actual Java source code and teach these objects new tricks. To do this, double-click the tan class boxes (like Square or Circle) to open the **Java Editor**.

## **🛑 Rules of the Matrix**

1. **Read Before You Type:** Look at how the other methods are written before you write your own.  
2. **Compile Often:** Every time you change the code, you must click the 🏗️ **Compile** button. If you get a red syntax error, you have to fix it before you can create any more objects\!  
3. **Save Your Work:** Remember the Ctrl \+ S shortcut.

## **😈 Boss 1: The Color Hacker (Estimated time: 30 mins)**

Right now, your shapes only accept a few colors (red, blue, yellow, green, magenta, black).

* **The Goal:** Add support for "orange" and "purple".  
* **The Clue:** The shapes don't actually control the colors. Double-click the Canvas class and look at the setForegroundColor method.  
* **The Task:** Write the Java else if statements to add the new colors. You will need to look up the RGB values for orange and purple\!

## **🐉 Boss 2: The Architect (Estimated time: 45 mins)**

Moving shapes horizontally and then vertically is slow. Let's make them move diagonally in one smooth action.

* **The Goal:** Open the Square class and write a brand new method called moveDiagonal().  
* **The Clue:** Look at how moveHorizontal() is written. Notice how it changes the xPosition.  
* **The Task:** Write a method that changes *both* the xPosition and yPosition at the exact same time, and *then* calls draw(). Test it by right-clicking a square on the object bench.

## **🌋 Boss 3: The Animator (Estimated time: 60+ mins)**

We have a slowMoveVertical method, but what if we want a shape to blink like a neon sign?

* **The Goal:** Open the Circle class and create a blink(int times) method.  
* **The Clue:** You will need to use a for loop (Google it or look at how slowMoveHorizontal uses one\!). Inside the loop, you need to make the circle invisible, wait a moment, make it visible, and wait again.  
* **The Task:** You will need to use Canvas.getCanvas().wait(500); to pause the code for half a second between blinks so your human eyes can see it.

## **🌌 Final Boss: The Morph**

*Only attempt if you have defeated the first three bosses.*

* **The Goal:** Open the Triangle class. Write a method called growAndShrink().  
* **The Task:** When called, the triangle should slowly increase its width and height by 50 pixels over a few seconds, and then slowly shrink back to its original size. You will need to combine loops, the changeSize() method, and the canvas wait() method.

> [!TIP]
>
> 🏆 **Bragging Rights:** If you complete the Final Boss, call the teacher over to show off your animation. You have officially written Quarter 3 level code in Week 1\!
