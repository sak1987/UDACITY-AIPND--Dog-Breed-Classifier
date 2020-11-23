# UDACITY-AIPND--Use a Pre-trained Image Classifier to Identify Dog Breeds
_**Project of AI Programming with Python Nanodegree by Udacity**_

![Dog Breeds](https://user-images.githubusercontent.com/33560386/99956735-f053b600-2d9f-11eb-9bb1-12724685b68e.JPG)

This is a very popular project across Machine learning & Artificial Intelligence Nanodegree Programs offered by [Udacity!](https://www.udacity.com/). This project requires working with three different pre-trained image classifiers. In addition, and writing our own script to identify different dog breeds.

## **Project Goal**
Improving our programming skills using **Python**.

## **Project Description**:
Your city is hosting a citywide dog show and you have volunteered to help the organizing committee with contestant registration. Every participant that registers must submit an image of their dog along with biographical information about their dog. The registration system tags the images based upon the biographical information.
Some people are planning on registering pets that aren’t actual dogs.

You need to use an already developed Python classifier to make sure the participants are dogs.

_**Note, you DO NOT need to create the classifier. It will be provided to you. You will need to apply the Python tools you just learned to USE the classifier.**_

## **Tasks:**

1. Using our Python skills, as we will determine which image classification algorithm works the "best" on classifying images as "dogs" or "not dogs".
2. Determine how well the "best" classification algorithm works on correctly identifying a dog's breed.
If the programmer are confused by the term image classifier look at it simply as a tool that has an input and an output. The Input is an image. The output determines what the image depicts.
(for example: a dog). Be mindful of the fact that image classifiers do not always categorize the images correctly. (We will get to all those details much later on the program).
3. Time how long each algorithm takes to solve the classification problem. With computational tasks, there is often a trade-off between accuracy and runtime. The more accurate an algorithm, the higher the likelihood that it will take more time to run and use more computational resources to run.

## **Principal Objectives**

1. Correctly identify which pet images are of dogs (even if breed is misclassified) and which pet images aren't of dogs.
 
2. Correctly classify the breed of dog, for the images that are of dogs.
 
3. Determine which CNN model architecture (ResNet, AlexNet, or VGG), "best" achieve the objectives 1 and 2.
 
4. Consider the time resources required to best achieve objectives 1 and 2, and determine if an alternative solution would have given a "good enough" result, given the amount of time each of the algorithms take to run.


# **TODO:**

**Edit program check_images.py**
- The **check_images.py** is the program file that you will be editing to achieve the four objectives above. This file contains a **main()** function that outlines how to complete this program through using functions that have not yet been defined. You will be creating these undefined functions in **check_images.py** to achieve the objectives above.

All of the TODOs are listed in check_images.py. You will find further elaborations and explanations for each, in the following concepts of this project.

If you feel that you need more guidance, please refer to the files ending with_hints.py. In the workspace you will find a hint file for each of the tasks.

## **Important notes:**

1. Before beginning the project please review the Frequently Asked Questions, FAQ, about the project.
2. This project and other lessons within the Nanodegree will be using a GitHub repository to store program files and other resources for this Nanodegree. To learn more about **GitHub**, please see the GitHub Lesson that's located within the **Extracurricular** (optional) section of this Nanodegree.
3. The **Project Workspace** is set up with the programs and files (like pet_images folder) you will need to complete the project.
4. The Python comments that begin with **# TODO:** in the **check_images.py** program indicates where you will need to change the code of the program. The **comments in check_images.py** will help you make the changes needed.
5. Function docstrings contain input parameters and return values, which were left to provide guidance. You are welcome to program these functions differently.
6. In **6. Timing Code to 19. Printing Results** we will provide additional guidance for programming the undefined functions and completing the check_images.py program. This information has been provided to help you through the process.

## **The information provides:**

Which **Lessons** to review regarding programming the undefined functions.
Details about the assignment's files (e.g. image files in pet_images folder, dognames.txt).
Details regarding using the classifier function in **classifier.py**.
Links to relevant python documentation.
Relevant example code.
You can use the functions within the program **print_functions_for_lab_checks.py** to check your code for sections **8. Command Line Arguments through 17. Calculating Results.** You will find this program within the Project Workspace and within the **GitHub repository.**

## **Program Outline**

1.**Time** your program
- Use Time Module to compute program runtime
2.Get program **Inputs** from the user
- Use command line arguments to get user inputs
3.**Create** Pet Images Labels
- Use the pet images filenames to create labels
- Store the pet image labels in a data structure (e.g. dictionary)
4.**Create** Classifier Labels and Compare Labels
- Use the Classifier function to classify the images and create the classifier labels
- Compare Classifier Labels to Pet Image Labels
- Store Pet Labels, Classifier Labels, and their comparison in a complex data structure (e.g. dictionary of lists)
5.**Classifying Labels** as "Dogs" or "Not Dogs"
- Classify all Labels as "Dogs" or "Not Dogs" using dognames.txt file
- Store new classifications in the complex data structure (e.g. dictionary of lists)
6.**Calculate** the Results
- Use Labels and their classifications to determine how well the algorithm worked on classifying images
7.**Print** the Results

_**You will need to repeat these tasks for each of the three image classification algorithms that are provided to you.**_
