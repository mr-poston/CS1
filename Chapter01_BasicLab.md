# **🛠️ Lab 1: The Shapes Canvas & Git Setup**

**Objective:** Today, you will configure your professional version control tools and build your first virtual scene using Object-Oriented Programming (OOP) in the BlueJ IDE.

**Readings to Complete First:** Chapter 1: The Visual World of Objects and Classes

## **📦 Part 1: Establishing Version Control**

Before we build anything, we need to set up our "Save Game" system using Git. You only have to do Step 1 once this entire year!

### **Step 1: Introduce yourself to Git**

1. Open your computer's Terminal (or Command Prompt / Git Bash).

2. Type the following command and press Enter (replace with your actual first and last name):
`git config --global user.name "Jane Doe"`

3. Type the following command and press Enter (replace with your school email):
`git config --global user.email "jane.doe@student.school.edu"`

### **Step 2: Initialize the Repository**

1. Download the `ShapesLab` project folder provided by your teacher and unzip it to your Documents folder.

2. In your Terminal, navigate to your new `ShapesLab` folder. (*Hint: You can often right-click the folder in your file explorer and select "Open Git Bash here".*)

3. Type the magic command to start tracking this folder:
`git init`

4. You should see a message saying "Initialized empty Git repository". **Take a screenshot of this message! You need it for your grade.**

## **🍔 Part 2: The Core Challenge - Building the House**

Now, let's create some Objects! Open the `ShapesLab` project in BlueJ. Your goal is to construct a simple house on the canvas by manually instantiating objects.

1. **The Wall:** Right-click the tan `Square` class and select `new Square()`. Name it `wall`.

2. **Make it Visible:** Right-click your new red `wall` object on the Object Bench and call the `makeVisible()` method.

3. **The Roof:** Right-click the `Triangle` class and instantiate a new triangle. Name it `roof`. Make it visible.

4. **The Sun:** Instantiate a `Circle` named `sun`. Make it visible.

5. **The Window:** Instantiate a second `Square` named `window`. Make it visible.

6. **Manipulate the State:**
Now, right-click your red objects and use their methods (`moveHorizontal`, `moveVertical`, `changeColor`, `changeSize`) to arrange them into a picture of a house with a sun in the sky.

    - *Note: If your roof is trapped behind your wall, remember that Java draws things in the order you made them visible! You might need to make the wall invisible and then visible again to bring it to the front.*

7. **Take a screenshot of your completed house on the Canvas!**

## **🌶️ Part 3: Spicy Extension - The Blueprint Coordinates**

*Finished early? Try this extension to prepare for next week's coding lab.*

Next week, you will have to type the exact Java code to make this house build itself automatically. You will need to know the exact math and coordinates for where every shape belongs.

1. Right-click your `sun` object and select **Inspect**.

2. Look at the variables. Write down the exact `xPosition`, `yPosition`, `size`, and `color` on a piece of scratch paper.

3. Do this for the `wall`, `roof`, and `window`.

4. Keep this paper in your folder. Next week, you will use these exact numbers to write your first script!

## **📥 Submission & Rubric**

To get credit for this lab, upload **two screenshots** to this Schoology assignment:

1. A screenshot of your Terminal showing the `git init` success message.

2. A screenshot of your BlueJ Canvas showing a completed house with at least 4 distinct, correctly positioned shapes.

| Category | Points | Description |
|---|---|---|
| Git Setup | 30 pts | Terminal screenshot proves git init was run in the correct folder. |
| Instantiation | 30 pts | Canvas screenshot shows at least 4 objects were successfully instantiated. |
| Method Calling | 40 pts | Canvas screenshot shows shapes were moved, resized, and colored correctly to resemble a house and a sun. |

> [!WARNING]
> 
> ⚠️ The "Blank Screen" Rule: Do not submit an empty assignment. If you get stuck on Git, submit the house. If you get stuck on the house, submit the Git screenshot. Partial credit is always better than a zero!
