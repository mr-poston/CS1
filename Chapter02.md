🖼️ Chapter 2: Source Code and the Automated House

In Chapter 1, you built a house by right-clicking, selecting new, and manually choosing methods from a menu.

While that visual tool is great for learning, it is incredibly slow. Imagine trying to build a video game with 10,000 trees by right-clicking 10,000 times! Real software engineers use Automation. Instead of doing the work themselves, they write a script—a list of written commands—that tells the computer how to do the work for them in a fraction of a second.

🕵️‍♂️ Inside the Java Editor

Remember the tan Class boxes (the blueprints) in BlueJ? If you double-click on one of those boxes, BlueJ will open a new window called the Java Editor.

This editor is basically a smart notepad. Inside, you will see lines of colorful text. This is Java Source Code. It is the actual language the computer reads to understand how to build and control your objects.

<img src="./images/JavaEditor.PNG" height="300" alt="Screenshot of the BlueJ Java Editor showing lines of colorful code inside the Picture class">




The Java Editor. Don't panic if it looks like an alien language right now!

Here is the basic "Grammar" you will see inside the editor:

🏰 The Castle Walls { }: Everything inside a Java class is enclosed in curly braces. If you open a {, you MUST close it with a }.

🛑 The Full Stop ;: Every single instruction you give the computer must end with a semicolon. It tells Java, "I am done with this command, move to the next line."

📝 The Comments //: Any line that starts with // is ignored by the computer. It is a sticky note left for human programmers to read.

🧩 The Anatomy of a Command (Syntax)

Programming languages have strict rules, just like English or Spanish. In English, a sentence must start with a capital letter and end with punctuation. In programming, these rules are called Syntax. If you break the syntax rules, the computer will completely refuse to run your program!

Let's look at the syntax for telling an object to perform a method in code:

sun.makeVisible();


Let's break down this "sentence" piece by piece:

The Object Name (sun): This is the Who. It tells Java exactly which object in its memory we want to talk to.

The Dot (.): This is the Command Operator. It connects the object to the action. You can read it out loud as "do this:".

The Method Name (makeVisible): This is the Action. It tells the object what behavior to perform. Notice the capitalization: the first word is lowercase, and the second word is capitalized. This is called camelCase, and it is the standard style for naming things in Java.

The Parentheses (): This is the How. Sometimes actions need extra details, called Parameters (like how far to move). Even if the action doesn't need extra details, you must include the empty parentheses so Java knows it's a method.

The Semicolon (;): This is the Period. It tells the computer that your command is finished.

[!CAUTION]
⚠️ The Syntax Monster: Java is case-sensitive! Typing wall.makevisible(); will cause a massive error because the 'v' is lowercase. It must be exactly makeVisible();! Missing semicolons and capitalization errors are the #1 cause of headaches for new programmers.

📜 Sequential Execution & Algorithms

When you write a script, you type your commands one after another, line by line.

wall.makeVisible();
wall.changeColor("blue");
roof.makeVisible();


When you tell the computer to run your script, it uses Sequential Execution. This means it reads your code exactly like a book: starting at the top, reading left to right, and moving down line by line. It will not execute line 3 until line 2 is completely finished.

A step-by-step list of instructions designed to solve a problem is called an Algorithm.

<img src="./images/SequentialExecution.PNG" height="300" alt="Graphic showing an arrow pointing down a list of code lines, demonstrating top-to-bottom reading">




The computer processes your algorithm one step at a time, strictly from top to bottom.

Order Matters!

Because computers execute code sequentially, the order of your algorithm is critical. If you tell Java to draw your roof before you tell it to draw the sky background, the sky will be drawn over your roof, completely hiding it! If your program isn't drawing things the way you expect, check the order of your commands.

📸 Git: Taking the Snapshot

Last week, we set up our version control and initialized our repository (git init). Git is now silently watching our folder.

However, as you type new code, Git does not automatically save your changes to the timeline. You have to explicitly tell Git to take a snapshot.

We do this in two steps:

1. Stage the changes (git add)

First, we tell Git which files we want to include in the snapshot.
We type: git add .
(The dot . is a shortcut that means "add every changed file in this folder to the stage").

2. Take the snapshot (git commit)

Next, we actually take the picture and add it to our timeline.
We type: git commit -m "Finished the walls and roof"
(The -m stands for message. You must leave a short, descriptive message about what you changed so you can find it later!)

<img src="./images/GitCommit.PNG" height="300" alt="Screenshot of a terminal showing a successful git add and git commit command">




A successful commit! Your code is now safely backed up in the version control timeline.

---

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
