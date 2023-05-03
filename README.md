Download Link: https://assignmentchef.com/product/solved-cs201-homework-2-coffee-quiz
<br>
<h1>Introduction</h1>

The aim of this homework is to practice on parametric functions and if statements. The use of if statement is necessary in this problem; however, the use of functions is required for good programming style. That means, it is possible to accomplish this homework without using functions, but it is a <u>must </u>to use them. The details about the use of functions in this homework are given later in this document.

<h1>Description</h1>

In this homework, you will write a C++ program that will help a barista know what kind of coffee customer would like to drink! Structured as a quiz program, your program will require the users to answer several questions based on ingredients used in making coffee, and notifies what kind of coffee has been prepared by the barista. After displaying a notification about this information, the program will close.

The user will be asked if they want certain ingredients in their coffee. The first question should be about espresso, if the user doesn’t want an espresso drink, then the answer is filtered coffee, and the program should close after displaying the proper notification. If the user prefers espresso, then your program will ask about the other ingredients. If your program has a match for the given ingredients, it should notify the user about the created coffee kind. This means, your program should not ask for every ingredient before displaying the notification – as it should be done when just the necessary information is already entered. For the relationship between ingredients and coffee kinds, you may find a coffee flowchart below in the functions section.

You may (and you should) find the exact notification format in the “Sample Runs” below.

We will be automatically grading your homeworks using GradeChecker, so it is very important to satisfy the exact same output given in the sample runs. You can utilize GradeChecker (<a href="http://sky.sabanciuniv.edu:8080/GradeChecker/">http://sky.sabanciuniv.edu:8080/GradeChecker/</a> ) to check whether your code is working in the expected way. To be able to use GradeChecker, you should upload all of your files used in the homework (<strong>only </strong>your_main_cpp file for this homework). Additionally, you should submit all of your files to SUCourse (<strong>only </strong>your main cpp file for this homework) <strong><u>without zipping </u></strong>them. <strong>Just a reminder, you will see a character ¶ which refers to a newline in your expected output.</strong>

<strong>The name of your main source (cpp) file should be in the expected format: </strong>“sucourseusername_lastname_name_hwnumber.cpp” (all lowercase letters). Please check the submission procedures of the homework in this document.

<strong>To get help using GradeChecker you may ask questions to the list of your grader TAs: <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5e3d2d6c6e6f393d363b322e1e32372d2a2d702d3f3c3f303d372b303728703b3a2b">[email protected]</a></strong>

<h1>Input Check</h1>

You are not expected to perform any input checks. You may assume, answers to the questions will be entered only as a “yes” or a “no”. Please be careful that answers are expected in lower-case.

<h1>Flow Chart</h1>

You may refer to Figure 1 for the flow of your program. Please note that this flow should be implemented using several functions in your program. Please refer to the functions section for details.

<strong>Figure 1 </strong>Flow Chart

<h1>Use of Functions (EXTREMELY IMPORTANT!)</h1>

<strong>You have to follow the specifications below for function declaration and callings. The grading criteria will include proper use of these parametric functions. Do NOT use any global variables (variables defined outside the functions) to avoid parameter use. Unnecessary code duplication will cause grade reduction as well.</strong>

In the first homework you were not supposed to implement any functions. However, in this homework <u>you are expected to </u>(actually <u>you have to</u>) use some function(s). The guidance about using functions in this homework is below.

A total of <strong>four </strong>user-defined functions (other than main) must be implemented. Two of these functions are void functions and two of them are non-void functions. You <u>have to </u>implement and use these four functions. If you don’t, your grade will be lowered because of the missing functions. On top of these functions, you may use other functions if you want.

The program flow will be as follows:

<ul>

 <li><strong>main function: </strong>You will display a welcome message, and then ask for the name of the customer. Then, you should proceed to function1 with name as its parameter. The same steps will be repeated for the other customer.</li>

 <li><strong>void function1(string): </strong>This function will be called from main with customer name as parameter, and it will call other given functions depending on program state. Asks the questions based on the flow chart given above. First question should be about espresso, for the rest of the questions you will construct the order. For the questions, you should make use of either function2 or function3. Note that if there were more than one customer, calling this function multiple times with appropriate parameters would have been enough.</li>

 <li><strong>bool function2(string): </strong>Prompts the user whether given ingredient is wanted or not. The string parameter will be an ingredient such as “foam” or “water”. When answered “yes”, this function returns true. When answered as “no”, this function returns false.</li>

 <li><strong>bool function3(string, string): </strong>Prompts the user whether the given 2 ingredients are in equal amounts or not. The string parameters will be ingredients such as “milk” or “foam”. When answered</li>

</ul>

“yes”, this function returns true. When answered as “no”, this function returns false.

<ul>

 <li><strong>void function4(string, string): </strong>Takes the name of the customer and resulting coffee kind as parameters, and displays a message using them.</li>

</ul>

Needless to say, you have to name these four functions using <strong><u>meaningful </u></strong>identifiers, not as Function1, Function2, etc.

<strong>No abrupt program termination please!</strong>

You may want to stop the execution of the program at a specific place in the program. Although there are ways of doing this in C++, it is not a good programming practice to abruptly stop the execution in the middle of the program. Therefore, your program flow should continue until the end of the main function and finish there.

<h2>Sample Runs</h2>

Below, we provide some sample runs of the program that you will develop. The italic and bold phrases are inputs taken from the user. You should follow the input order in these examples and the prompts your program will display must be <strong>exactly the same </strong>as in the following examples.

<h3>Sample Run 1</h3>

Welcome to Pequod’s Coffee! Can you tell me your name?

<h4>Robert</h4>

Dear Robert, would you kindly answer our questions, so we can determine the coffee you want. Does it have espresso? <strong><em>no</em></strong>

Your order is ready Robert! What you want is a filtered coffee. Enjoy!

<h3>Sample Run 2</h3>

Welcome to Pequod’s Coffee! Can you tell me your name?

<h4>Alan</h4>

Dear Alan, would you kindly answer our questions, so we can determine the coffee you want. Does it have espresso? <strong><em>yes</em></strong>

Does it have milk? <strong><em>yes</em></strong>

Does it have hot chocolate? <strong><em>no</em></strong>

Does it have foam? <strong><em>no</em></strong>

Your order is ready Alan! What you want is a cafe au lait. Enjoy!

<h3>Sample Run 3</h3>

Welcome to Pequod’s Coffee! Can you tell me your name?

<h4>Jesse</h4>

Dear Jesse, would you kindly answer our questions, so we can determine the coffee you want. Does it have espresso? <strong><em>yes</em></strong>

Does it have milk? <strong><em>yes</em></strong>

Does it have hot chocolate? <strong><em>no</em></strong>

Does it have foam? <strong><em>yes</em></strong>

Do foam and milk are in equal amounts? <strong><em>yes</em></strong>

Your order is ready Jesse! What you want is a cappucino. Enjoy!

<h3>Sample Run 4</h3>

Welcome to Pequod’s Coffee! Can you tell me your name?

<h4>Ronaldo</h4>

Dear Ronaldo, would you kindly answer our questions, so we can determine the coffee you want. Does it have espresso? <strong><em>yes</em></strong>

Does it have milk?

<h5>no</h5>

Does it have water? <strong><em>yes</em></strong>

Your order is ready Ronaldo! What you want is an americano. Enjoy!


