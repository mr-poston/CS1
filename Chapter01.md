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
