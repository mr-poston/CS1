# **🖼️ Chapter 2: The Picture Class (Writing Your First Script)**

Last week, you built a house by manually clicking on objects and calling methods like `moveRight()`. If you wanted to build it again, you had to click everything all over again.

Real programmers don't like repeating themselves. Instead, they write a **Script**—a set of instructions that the computer remembers and runs automatically. Today, we open the Java Editor\!

## **⏱️ Weekly Pacing Guide (\~4 Hours)**

* **Block 1 (90 mins):** Anatomy of the Java Editor, declaring variables, and instantiating objects in code.  
* **Block 2 (90 mins):** Lab 2.1 (Scripting the House).  
* **Block 3 (45-90 mins):** Lab 2.2 (The Sunset Animation) & Spicy Extensions.

## **📝 2.1 Inside the Java Editor**

In your BlueJ project, double-click the tan Picture class. This opens the **Java Editor**. Let's look at the basic "Grammar" of Java:

### **🏰 The Castle Walls `{ }`**

Everything inside a Java class is enclosed in curly braces `{ }`. If you open a `{`, you MUST close it with a `}`.

### **🛑 The Full Stop `;`**

Every single instruction you give the computer must end with a semicolon `;`. It tells Java, "I am done with this command, move to the next line."

### **📝 The Comments `//`**

Any line that starts with `//` is ignored by the computer. It is a sticky note left for human programmers to read.

## **🏗️ 2.2 The Three Steps of Object Creation**

To make a shape appear using pure code, you have to follow three steps inside the Picture class.

**1\. Declare the Variable (The Box):**

First, we tell the computer to reserve a space in memory for our shape. We put this at the top of the class.

```java
private Square wall; // 📦 We want a Square, and we will call it "wall"
```

**2\. Instantiate the Object (The Contents):**

Next, we actually build the shape using the new keyword. We put this inside the *Constructor* (the setup method).

```java
wall = new Square(); // 🪄 Poof! The object is created in memory.
```

**3\. Call the Methods (The Action):**

Finally, we tell the object what to do. We put this inside the draw() method.

```java
wall.makeVisible(); // 👁️ Show it on the canvas!  
wall.changeColor("blue"); // 🎨 Change the color.  
wall.moveHorizontal(50); // ➡️ Move it to the right.
```

## **🛠️ Lab 2: Scripting the Canvas**

### **🍔 Lab 2.1: The Core Challenge \- "The Automated House"**

Your goal today is to write the Java code that automatically draws the house you built by hand last week.

1. Open the Picture class in the BlueJ editor.  
2. Scroll down to the `draw()` method.  
3. You will see some code is already there. Delete it, and write your own instructions to build:  
   * A "blue" square for the wall.  
   * A "green" triangle for the roof.  
   * A "yellow" circle for the sun.  
   * *Hint: You will need to use moveHorizontal and moveVertical to position them correctly\!*  
4. 🏗️ **Compile** your code. Fix any missing `;` or `{` errors.  
5. Go back to the BlueJ main screen, right-click Picture, select `new Picture()`, and then call the `draw()` method on the red object. Watch your house draw itself instantly\!

### **🍔 Lab 2.2: The Sunset Animation**

Let's make it move\!

1. Add a new method inside your Picture class called `sunset()`.  
2. Inside this method, write code that tells your sun object to `slowMoveVertical()` down behind the house.  
3. Call `sun.changeColor("orange");` halfway through the method so the sun changes color as it sets\!

> [!CAUTION]
>
> ⚠️ **The Syntax Monster:** Java is case-sensitive\! wall.makevisible(); will cause a massive error because the 'v' is lowercase. It must be exactly makeVisible();\!
