# UDACITY- AIPND- Use a Pre-trained Image Classifier to Identify Dog Breeds.
This repository contains _REVISED_ code and associated files for the AI Programming with Python Nanodegree program. This repository consists of a number of tutorial notebooks for various coding exercises and programming labs that will be used to supplement the lessons of the course.

## _**Intro to Python Project - Classifying Pet Images**_

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

- Which **Lessons** to review regarding programming the undefined functions.
- Details about the assignment's files (e.g. image files in pet_images folder, dognames.txt).
- Details regarding using the classifier function in **classifier.py**.
- Links to relevant python documentation.
- Relevant example code.
- You can use the functions within the program **print_functions_for_lab_checks.py** to check your code for sections **8. Command Line Arguments through 17. Calculating Results.** You will find this program within the Project Workspace and within the **GitHub repository.**

## **Program Outline**

1.**Time** your program
- Use Time Module to compute program runtime
2. Get program **Inputs** from the user
- Use command line arguments to get user inputs
3. **Create** Pet Images Labels
- Use the pet images filenames to create labels
- Store the pet image labels in a data structure (e.g. dictionary)
4. **Create** Classifier Labels and Compare Labels
- Use the Classifier function to classify the images and create the classifier labels
- Compare Classifier Labels to Pet Image Labels
- Store Pet Labels, Classifier Labels, and their comparison in a complex data structure (e.g. dictionary of lists)
5. **Classifying Labels** as "Dogs" or "Not Dogs"
- Classify all Labels as "Dogs" or "Not Dogs" using dognames.txt file
- Store new classifications in the complex data structure (e.g. dictionary of lists)
6. **Calculate** the Results
- Use Labels and their classifications to determine how well the algorithm worked on classifying images
7. **Print** the Results

_**You will need to repeat these tasks for each of the three image classification algorithms that are provided to you.**_

## Issues with the Project Workspace
- While it is recommended that you work on the project within the **_Project Workspace_**, a few students _may_ experienced issues trying to work within the _Project Workspace_.  Some students found these issues resolved when they switched their internet browsers.  Specifically, some students found that **_Chrome_** worked best; while others found that **_Firefox_** worked better for them.  If you are running into the problem where the _files_ in the workspace don't load and/or running code within the workspace runs extremely slowly; please try the following:
* Quit and exit out of the **_web browser_** you are using, then open it back up and restart it.
* Switch to a different **_web browser_**. 

- If you **run into issues** with the **_Project Workspace_** and the above recommendations didn't work; alternativIy, you are welcome to complete the project on a local computer using the instructions in the next [FAQ](https://github.com/udacity/AIPND-revision/blob/master/notes/project_intro-to-python.md#running-the-project-on-a-local-computer). 

## Files Required to Run **_check_images.py_** Locally
The following files and folders need to be put in the same folder as the **_check_images.py_** python program on your local computer. You will find these files and folders within the [GitHub AIPND Repository](https://github.com/udacity/AIPND-revision/tree/master/intropyproject-classify-pet-images). There are more programs in the repository than you will need, these extra programs are there to provide the code within the lessons in a format that can be copied and pasted from.
### Needed Files:
* **pet_images**  (folder of 40 pet image)
* **uploaded_images** (a folder you will have to create to hold your uploaded images in that section of the project)
* **classifier.py** (classifier function you will be using to classify the images)
* **dognames.txt** (file that contains all the valid dog names from the classifier function and the pet image files)
* **imagenet1000_clsid_to_human.txt** (dictionary that converts the classifier function ids to text labels)
* **adjust_results4_isadog.py** (a program that contains the **adjust_results4_isadog** function that you will be defining as part of the project)
* **calculates_results_stats.py** (a program that contains the **calculates_results_stats** function that you will be defining as part of the project)
* **classify_images.py** (a program that contains the **classify_images** function that you will be defining as part of the project)
* **get_input_args.py** (a program that contains the **get_input_args** function that you will be defining as part of the project)
* **get_pet_labels.py** (a program that contains the **get_pet_labels** function that you will be defining as part of the project)
* **print_results.py** (a program that contains the **print_results** function that you will be defining as part of the project)
* **run_models_batch.sh** (a bash script that will run check_images.py sequentially for all 3 model architectures and output their results to text files - on Unix/Linux/OSX/Project Workspace from a terminal window)
* **run_models_batch.bat** (a batch script that will run check_images.py sequentially for all 3 model architectures and output their results to text files - on Windows from the Anaconda Prompt window)
* **run_models_batch_uploaded.sh** (a bash script that will run check_images.py sequentially for all 3 model architectures  on the uploaded images folder and output their results to text files - on Unix/Linux/OSX/Project Workspace from a terminal window)
* **run_models_batch_uploaded.bat** (a batch script that will run check_images.py sequentially for all 3 model architectures on the uploaded images folder and output their results to text files - on Windows from the Anaconda Prompt window)
* **test_classifier.py** (an example program that demonstrates how to use the classifier function)
* **print_functions_for_lab_checks.py** (a program that contains functions that will allow you to check your code)

**Also be aware that instructor provided **_hints_** files are provided for each of the functions used within this project, these files will end with **_hints.py**. These **_hints_** files contain extra code to provide a few **_hints_** to help guide students to the solution. You will find these **_hints_** files within the **_Project Workspace_** and also within the [**_GitHub repository_**](https://github.com/udacity/AIPND-revision/tree/master/intropyproject-classify-pet-images) as the following files:

* **adjust_results4_isadog_hints.py** (a program that contains **_hints_** for the **adjust_results4_isadog** function that you will be defining as part of the project)
* **calculates_results_stats_hints.py** (a program that contains **_hints_** for the **calculates_results_stats** function that you will be defining as part of the project)
* **classify_images_hints.py** (a program that contains **_hints_** for the **classify_images** function that you will be defining as part of the project)
* **get_input_args_hints.py** (a program that contains **_hints_** for the **get_input_args** function that you will be defining as part of the project)
* **get_pet_labels_hints.py** (a program that contains **_hints_** for the **get_pet_labels** function that you will be defining as part of the project)
* **print_results_hints.py** (a program that contains **_hints_** for the **print_results** function that you will be defining as part of the project)
&nbsp;   
&nbsp;     
     
## Running Batch Files on Windows OS Locally
- To run the files **_run_models_batch_** or **_run_models_batch_uploaded_** that run all 3 model architectures using **_check_images.py_** on a Windows OS locally; you will need to use the files that end with the extention **_.bat_** instead of the extension **_.sh_**.  You will have also needed to have installed Anaconda on your computer (see following [FAQ](https://github.com/udacity/AIPND-revision/blob/master/notes/project_intro-to-python.md#running-the-project-on-a-local-computer) for details on Anaconda installation).
### Directions:
* Open the **Anaconda Prompt** - either from typing **_Anaconda Prompt_** within the search bar and selecting it _or_ by clicking on it once it's found within the **Anaconda** folder of programs.
* Navigate to the _folder_ within the **Anaconda Prompt** that contains the _Project files_ including **_check_images.py_** and **_run_models_batch.bat_** using the command [_cd_](https://en.wikipedia.org/wiki/Cd_(command)).
* Type the command within the **Anaconda Prompt**:
```terminal
run_models_batch.bat
```
- If instead you are working with the uploaded images , you will replace all instances of **_run_models_batch.bat_** from the _directions_ above with **_run_models_batch_uploaded.bat_**. 
&nbsp;     
&nbsp;         

## **_Hints_** for this Project
Instructor provided **_hints_** files are provided for each of the functions used within this project, these files will end with **_hints.py**. These **_hints_** files contain extra code to provide a few **_hints_** to help guide students to the solution. You will find these **_hints_** files within the **_Project Workspace_** and also within the [**_GitHub repository_**](https://github.com/udacity/AIPND-revision/tree/master/intropyproject-classify-pet-images) as the following files:   
* **adjust_results4_isadog_hints.py** (a program that contains **_hints_** for the **adjust_results4_isadog** function that you will be defining as part of the project)
* **calculates_results_stats_hints.py** (a program that contains **_hints_** for the **calculates_results_stats** function that you will be defining as part of the project)
* **classify_images_hints.py** (a program that contains **_hints_** for the **classify_images** function that you will be defining as part of the project)
* **get_input_args_hints.py** (a program that contains **_hints_** for the **get_input_args** function that you will be defining as part of the project)
* **get_pet_labels_hints.py** (a program that contains **_hints_** for the **get_pet_labels** function that you will be defining as part of the project)
* **print_results_hints.py** (a program that contains **_hints_** for the **print_results** function that you will be defining as part of the project)
&nbsp;   
&nbsp;   

## Eliminating Syntax Errors with Text Editor/Integrated Development Environment 
- If you are experiencing a lot of syntax errors with your code, you may consider downloading your code and looking at it with your favorite text editor/IDE to help eliminate the syntax errors from your program.  Recall in **_2. Intro to Python_**, **_Lesson 5. Scripting_**, **_Section 6. Programming Environment Setup_** you were provided with a number of text editors that are available to use with python (like _Atom_, _Sublime Text_, _Notepad++_). Additionally, when you installed Anaconda, the Spyder IDE (Integrated Development Environment) for python should be available through the _Anaconda Navigator_. 
&nbsp;   
&nbsp;   
     
## Cutting and Pasting Code in the Classroom
- If you cut and paste code directly from the classroom, it is very likely you will generate syntax errors with the single and double quotes. This is because the font type differences.  If you are going to cut and paste code from the classroom, you will need to erase and replace any copied double or single quotes.  Additionally, cutting and pasting code from the classroom may also result in issues regarding the proper code indention; therefore, it is not recommended to cut and paste code directly from the classroom.
&nbsp;    
&nbsp;   
     
## Indention of Python Code
- Indention is used within Python to distinquish between blocks of code; whereas, with other programming languages, like Java and  C++,  they may have used curly brackets. The [PEP8 Style guide](https://www.python.org/dev/peps/pep-0008/) provides the standard for python code and is what has been used for the programs within the Github respository and the Project workspace. The [PEP8 standard for indention](https://www.python.org/dev/peps/pep-0008/#indentation) is to use 4 spaces for each indention level. Not using 4 spaces for indention when editing **_check_images.py_**, will likely result in syntax errors. 

- Be aware that using the **_tab_** key within most text editors might not guarentee the proper 4 space indention.  Additionally, not all text editors (including the **_Project Workspace_**) provide the proper 4 space indention as is used in the python programs within the repository for this project.
&nbsp;     
&nbsp;    
    
## Replacing None and Pass Statements
When editing the functions provided in **_check_images.py_** you will need to replace [_None_](https://docs.python.org/3/library/constants.html#None) or the [_pass_](https://docs.python.org/3/tutorial/controlflow.html#pass-statements) statement with your code for that function. The pass statement does nothing, it's used so that the program will still run eventhough the functions have not been fully defined. Similarly the value of _None_ represents the absence of a value, it's used so that the program will still run eventhough the functions have not been fully defined.
&nbsp;    
&nbsp;
