# **👾 Chapter 2 Boss Battles: Hacking the Picture**

*So, you finished the Automated House script and the Sunset animation? Time to level up. For these challenges, you will need to add new variables and learn some advanced syntax.*

## **🛑 Rules of the Matrix**

1. **No Errors Allowed:** Your code must compile cleanly 🏗️ before you ask the teacher to check your work.  
2. **Comment Your Code:** Use // to explain what your advanced code is doing.

## **😈 Boss 1: The Landscape Artist (Estimated time: 30 mins)**

A house on a blank white canvas is boring. Let's add some scenery.

* **The Goal:** Add a grass field and a background sky.  
* **The Task:** You must declare two new Square variables (e.g., sky and grass). In your draw() method, make the sky blue and the grass green.  
* **The Trick:** You will need to use the changeSize() method with a massive number (like 500\) to cover the whole screen.  
* **The Trap:** Java draws things in order\! If you draw the sky *after* you draw the house, the sky will paint right over the top of your house and hide it\! You must draw the background first.

## **🐉 Boss 2: Previewing Parameters (Estimated time: 45 mins)**

Right now, you have one draw() method that draws the house in a fixed spot. Let's write a method that lets the user choose where the sun goes\!

* **The Goal:** Write a new method called drawCustomSun(int x, int y).  
* **The Clue:** Notice the int x, int y inside the parentheses 📥? These are called **Parameters**. They allow the user to pass numbers into your method.  
* **The Task:** Inside this method, write the code to create a sun, but instead of using a specific number like moveHorizontal(50), use your new variables: sun.moveHorizontal(x); and sun.moveVertical(y);.  
* **Test it:** Go back to the BlueJ bench, right-click your Picture object, select drawCustomSun, and type in 100, 200 to see if it works\!

## **🌋 Boss 3: The Starry Night (Estimated time: 60+ mins)**

*Warning: This requires Googling concepts from Quarter 3 & 4\!*

* **The Goal:** Write a method called nightTime() that instantly changes the sky to black, the sun to a white moon, and generates 50 randomly placed white stars in the sky.  
* **The Clue:** You do *not* want to type out 50 Circle variables. You need a for loop.  
* **The Task:** 1\. Look up how to write a Java for loop that counts from 1 to 50\.  
  2\. Look up Math.random().  
  3\. Inside the loop, instantiate a new Circle(), make it white, shrink it down to size 5, and use Math.random() to generate random x and y coordinates to move it to.

\[\!TIP\]

🏆 **Bragging Rights:** If you complete The Starry Night, you have officially mastered Loops and Randomization weeks before the rest of the class. Show the teacher\!
