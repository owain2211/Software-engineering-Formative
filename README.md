# Software-engineering-Formative

### What the code does
The code is an app which allows the user to either multiply or add two numbers, with the answer printed for the user within the app, it is written in python and makes use of the tkinter package, which provides all the functions to create a graphical user interface

### How the code was developed

* The first step was two decide what the app should do
* Next an intial design of what the app should look like was created
* After this a "dummy" version of the app could was created
* Once the "dummy" version looked right the functions which the buttons execute needed to be designed
* Next, the functionality was added to the buttons
* Finally. the app was tested

The progress of the app was tracked using a kanban board which can be seen below


![Alt text](https://github.com/owain2211/Software-engineering-Formative/blob/a7443db8c41cc5b5c590f37c0fc93265c3a2cf2e/Kanban%20board%20for%20formative.png)

The kanban board shows the project while the function which calculates the results after the button is clicked was being tested. The final item in the to do section is still incomplete at the moment.

### How to use the app

The app is designed to be simple to use, with only a single button and three data entry points, the final app along with the different features can be seen in the below

![Alt text](https://github.com/owain2211/Software-engineering-Formative/blob/9ee2be1784a6fd85b6cae8e67f6f74895b3e0726/app_layout.jpg)

If the user hasn't entered/selected data in any of the three data entry boxes then an error message will appear when the button is clicked and the boxes will be cleared, an error also appears if text is entered in either of the number boxes.

### The code

The GUI class has to functions, the first is the __init__ function which runs the graphical user interface whent the code is run, within this function all the variables are defined such as the two numbers and the colours of the app and in addition the shape and look of the app is defined as the frames are created, and then the buttons and entry boxes are created and added to the frames, the positioning of the items within the frames is done using a grid method .

The second function is the one used to calcualte the answer to the sum its given, this function runs when the button is clicked. It first checks whether the two numbers are numeric and that the combo box isn't empty, if this test fails then the below error message appears.

![Alt text](https://github.com/owain2211/Software-engineering-Formative/blob/9ee2be1784a6fd85b6cae8e67f6f74895b3e0726/app_error_message.jpg)

If the conditions are met then it converts the two input numbers to ints, and then based on whether addition or multiply has been selected it will add or mutliply the numbers to generate an answer and also set the operation to  + or *, this is so that the equation in full can be printed to the user. Next a string of the equation is created in the format of number_1 operation number_2 = answer i.e it could be 1 + 2 = 3. Once the result has been created the variable which the answer box displays is set to the result and the two number entry boxes are cleared, meaning the equation the user defined along with the answer is displayed to them.

