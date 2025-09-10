# JavaApplication1

Vanier College - Computer Science & Mathematics
Program Development in a Graphical Environment
Lab_02- Fall 2025
Due: end of the class Prof.: Nagat Drawel
Instructions:
1. Please submit one .java file 
2. Use Git throughout your development process, make regular commits with descriptive 
commit messages and include the link to your Git repository as a comment at the top of 
your .java file.
What to Do
Write a JavaFX application that meets the following requirements:
• Use a BorderPane as the root layout. A BorderPane has five regions: Top, Bottom, Left, 
Right, and Center.
• In the Top region, add a Label that displays: “Random Game”.
• In the Bottom region, add a Label that displays: “Waiting…”.
• In the Left and Right regions, leave them empty (or optionally add placeholder Labels for 
testing).
• In the Center region, add a Label to display the game image. Place this Label inside a 
StackPane, then add the StackPane to the Center of the BorderPane.
• The image should be loaded randomly by generating a random number (using the 
Random class) and constructing the filename.
• There are 20 images named 101.png through 120.png. These images are provided in the 
zip file attached to this lab.
Getting Started
1. Create the Project
o Create a new JavaFX project in NetBeans.
o Name the project: Lab02_YourName.
2. Set Up the Stage (inside the start method)
o Create a BorderPane called root.
o Create a new Scene using root as the layout, with a width of 250 and a height of 
300.
o Set the stage title to “Java Games”.
o Call primaryStage.show().
o At this point, you should see an empty window running.
3. Add the Images Folder
o Download and unzip the provided images.
o Place them in a folder named images inside your project root.
o Your project structure should look like this: 
▪ build 
▪ test 
▪ nbproject 
▪ src 
▪ images <- place the 20 .png files here
Building the Layout
1. Create a StackPane called middle.
2. Create a Label for the Top (e.g., “Random Game”).
3. Create a Label for the Bottom (e.g., “Waiting…”).
4. Create a Label named lblImage (blank at the start).
5. Add the Top Label to the Top region of the BorderPane.
6. Add the Bottom Label to the Bottom region of the BorderPane.
7. Add lblImage to the StackPane middle, then add middle to the Center of the 
BorderPane.
At this point, your window should have all the Labels in place, but no image is shown yet.
Loading a Random Image
1. Import the required packages: import javafx.scene.image.*; import java.util.Random;
2. The images are named 101.png through 120.png. Use Random to generate a number 
between 101 and 120
3. Construct the file path using string concatenation by inserting the random number into 
the image name.
4. Create an Image object using this path
5. Set the image on your Label (lblImage) as a graphic: lblImage.setGraphic(new 
ImageView(img));
Now, each time you run the application, a random image from 101.png to 120.png should 
appear in the Center of the BorderPane.
