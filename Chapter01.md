# **📖 Chapter 1: The Visual World of Objects and Classes**

Welcome to Computer Science 1! This year, you are going to learn how to write software using **Java**, one of the most popular programming languages in the world. Java is used to build Android apps, enterprise web servers, and even games like *Minecraft*.

Before we write lines of code, we need to understand *how* Java thinks. Java is an **Object-Oriented Programming (OOP) language**. This means that instead of just writing a long list of math commands, we design virtual "Objects" that interact with each other.

## **🏛️ Classes vs. Objects**

The two most important words in this course are **Class** and **Object**.

Imagine you want to build a neighborhood. You wouldn't just start nailing wood together randomly. First, you need an architect to draw a **Blueprint**. The blueprint isn't a physical house—you can't open its doors or sleep in its bedrooms. It is just a design. However, once you have that blueprint, builders can use it to build as many physical **Houses** as needed.

In Java:

- A **Class** 🗺️ is the Blueprint. It is the code that defines what something is and what it can do.
- An **Object** 🏠 is the physical House. It is the actual, usable thing created from the Class.
- We call the process of building an object **Instantiation** 🏗️ (creating an instance of a class).

> [!NOTE]
> *Analogy Check: If "Cookie Cutter" is the Class, then the "Cookie" is the Object!*

## **💻 The BlueJ Environment**

To write and test our Java code, we use a tool called an **IDE** (Integrated Development Environment) named BlueJ. BlueJ is special because it lets us see our Classes and Objects visually before we start typing code.

### **1. The Class Diagram**

When you open a project in BlueJ, the large main window is the Class Diagram.
You will see tan-colored boxes. Each of these boxes represents a Class (a blueprint) that a programmer has already written for you.

<img src="./images/ClassDiagram.PNG" height="300" alt="Screenshot of the BlueJ main window showing the tan boxes for Circle, Square, Triangle, and Canvas"><br>
*The tan boxes are Classes. Notice the arrows showing how they connect to the Canvas.*

### **2. The Object Bench**

At the bottom of the BlueJ window is a red area called the Object Bench. When you right-click on a tan Class box and select `new`, you are telling Java to *instantiate* an Object. The new Object will appear as a red box on the Object Bench.

<img src="./images/ObjectBench.PNG" height="300" alt="Screenshot of the BlueJ Object Bench at the bottom of the screen with a few red shape objects sitting on it"><br>
*The red boxes are Objects. They have been built from the blueprints and exist in the computer's memory.*

## **📦 State and Behavior 🏃‍♂️**

Once you have an Object sitting on your Object Bench, what can you do with it? Every object in Java has two main characteristics: **Behavior** and **State**.

### Behavior (Methods) 🏃

Objects can do things. These actions are called **Methods**. Think of Methods as the "Verbs" of programming.
If you have a `Square` object, its methods might include `moveRight()`, `changeColor()`, or `makeVisible()`. You can tell an object to perform an action by right-clicking the red object box and selecting the method from the menu.

### State (Fields / Variables) 📦

Objects also know things about themselves. This is called the object's **State**, and it is stored in **Variables** (also called Fields). Think of State as the "Adjectives" or "Nouns".
A `Square` object knows its `size`, its `xPosition`, its `yPosition`, and its `color`.

In BlueJ, you can spy on an object's state! If you right-click a red object and select **Inspect**, BlueJ will open a window showing you the exact values saved inside that object's memory.

<img src="./images/ObjectInspector.PNG" height="300" alt="Screenshot of the BlueJ 'Object Inspector' window showing variables like xPosition = 210, color = 'green'"><br>
*The Object Inspector reveals the hidden variables (State) stored inside the object.*

# 💾 Welcome to Git: The "Save Game" for Code

In this class, we won't just learn how to code; we will learn how professional engineers manage their projects using a tool called **Git**.

**What is Version Control?**
Have you ever worked on an essay and saved it as `essay_final.docx`? Then you made a change and saved it as `essay_final_v2.docx`? By the end, your folder is a mess of files like `essay_ACTUAL_FINAL_I_SWEAR.docx`.

Git solves this. Git is a **Version Control System**.
Think of Git like the "Save Game" feature in a video game. Instead of making hundreds of copies of your files, Git takes a "snapshot" of your folder at a specific moment in time. If you mess up your code and break your program, you can use Git to travel back in time and load your last working snapshot.

In this course, you will learn the commands to take these snapshots (`git add` and `git commit`), ensuring you never lose your hard work!


# **📦 Chapter 1: Objects, Classes, and the BlueJ Grid**

Welcome to Computer Science 1\! Before we start typing lines of code, we need to understand how Java "sees" the world. Java is an **Object-Oriented** programming language. That means it builds programs by creating virtual "objects" that interact with each other.

To see these objects, we use a special program called **BlueJ**.

## **⏱️ Weekly Pacing Guide (\~4 Hours)**

* **Block 1 (90 mins):** Intro to Objects, BlueJ Interface Tour, Lab 1.1 (Single Shapes).  
* **Block 2 (90 mins):** Lab 1.2 (Building the House) & State Inspection.  
* **Block 3 (45-90 mins):** Lab 1.3 (The Neighborhood) & Spicy Extensions.

## **🏗️ 1.1 The Blueprint vs. The Building**

In programming, we have to distinguish between the *idea* of a thing and the *actual* thing.

* 📘 **A Class** is the blueprint. It is a set of instructions that describes how to build something. (Think: A cookie cutter).  
* 🍎 **An Object** is the actual thing built from the blueprint. (Think: The physical cookie you can eat).  
* 📝 **Java Vocab:** When we create a new object from a Class, we call it an **Instance**.

If you have a Class called Student, you only need *one* blueprint. But you can use that blueprint to create 30 unique Student **Objects** (one for each person in our classroom).

## **🗺️ 1.2 Navigating the BlueJ Grid**

When you open a project in BlueJ, you will see a big blank grid with some colored rectangles on it. Let's break down the map:

1. **The Grid (Main Window):** This is where your **Classes** live. You will usually see them represented as tan or orange rectangles.  
2. **The Arrows:** The dashed lines between the classes show relationships. If a House class points to a Square class, it means the House *uses* Squares to build itself.  
3. **The Object Bench (The Red Zone):** Look at the very bottom of the screen. It’s an empty gray bar. This is where your **Objects** will live once you create them.

## **🪄 1.3 Conjuring Objects into Existence**

Let's make something happen\!

1. Right-click on the tan Circle class.  
2. Select new Circle().  
3. A popup will ask you for a name (the "Instance Name"). You can leave it as circle1 or name it sun.  
4. Click OK.

**Look at the Object Bench\!** A red rectangle just appeared at the bottom of your screen. You just used the Circle blueprint to instantiate a real Circle object in the computer's memory\!

### **🕹️ Giving Commands (Methods)**

Your object exists, but you can't see it yet. Let's tell it what to do.

Right-click your red object on the bottom bench. This menu shows you all the **Methods** (actions/verbs) this object knows how to do.

* Right-click the red object ![][image1] select makeVisible().  
* A new window will pop up showing your circle\!  
* Right-click the red object again ![][image1] select moveRight(). Watch it jump\!

## **🛠️ Lab 1: The Shapes Canvas**

### **🍔 Lab 1.1: The Warmup (Block 1\)**

1. Open the shapes project in BlueJ.  
2. Create one of each shape (Circle, Square, Triangle).  
3. Make them all visible.  
4. Practice using moveRight(), moveDown(), and changeColor() to spread them out on the canvas so they don't overlap.  
   *Allowed colors: "red", "yellow", "blue", "green", "magenta", "black".*

### **🍔 Lab 1.2: The Core Challenge \- "The House" (Block 2\)**

Your goal today is to manually build a simple picture by creating objects and giving them commands.

1. Create a Square object. Make it visible, and change its color to "blue" (make sure to include the quote marks\!) to act as the walls of a house.  
2. Create a Triangle object. Make it visible, change its color to "green", and move it so it sits on top of the square as a roof.  
3. Create a Circle object. Make it visible, change its color to "yellow", and move it into the sky to be the sun.

> [!CAUTION]
>
> ⚠️ **The "Vanish" Act:** If you close BlueJ, your classes (the tan boxes) will save, but your **Objects** (the red boxes) will disappear\! Objects only live in the computer's temporary memory (RAM). When you restart BlueJ, you have to build them again\!

### **🍔 Lab 1.3: The Neighborhood (Block 3\)**

Can you scale your design?

1. Build *two* houses side-by-side.  
2. **Wait, it's taking forever to click?** Right-click your objects and look for methods that take **Parameters** 📥.  
3. Try using moveHorizontal(int distance). Type 100 into the box instead of clicking moveRight() ten times\!

### **🌶️ The Spicy Extensions**

*For students who finish the Core Challenges early, or for those who want to push their AP logic skills.*

1. **The Inspector:** Right-click your sun (Circle) object and select **Inspect**. This shows you the object's **State** (its hidden variables like xPosition and yPosition).  
2. **The Smooth Animation:** Instead of using moveRight(), right-click and find the method slowMoveVertical(). Type in a number like 150 and hit enter. What happens?  
3. **The Eclipse:** Create a second circle. Make it "black". Without looking at the canvas (only looking at the **Inspect** window for both circles), figure out exactly what numbers you need to type into moveHorizontal() and moveVertical() to make the black circle perfectly overlap the yellow sun to create a total solar eclipse.
