Download Link: https://assignmentchef.com/product/solved-cs135-project-7
<br>
<u>Project [7]: Pointers</u>




<strong>Project Goals </strong>

The goal of this project is to:

<ol>

 <li>Get students familiar with the use of pointers</li>

</ol>




<strong><u>Important Notes:</u> </strong>

<ol>

 <li><strong>Formatting: </strong>Make sure that you follow the precise recommendations for the output content and formatting: for example, do not change the text of the problem from “Please type the real component: ” to “Enter real part: ”. Your assignment will be auto-graded and any change in formatting will result in a loss in the grade.</li>

 <li><strong>Comments: </strong>Header comments are required on all files, for each function, and recommended throughout the rest of the program. Points will be deducted if no header/function comments are included.</li>

 <li><strong>Restriction: </strong>The use of goto statements anywhere within this program is prohibited. Points will be deducted if gotois used.</li>

</ol>

<strong> </strong>




<strong>Problem 1 </strong>

Write a program that adds, subtracts, and multiplies complex numbers. This program will prompt the user for the choice of operation, read in the complex numbers, perform the operation, and print the result. Your program must use the six functions described below.

At the beginning, the program should output the following:

Complex Number Arithmetic Program:

At every iteration, your program should ask the user for an option as follows:

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Quit</li>

</ul>

<h1>Choose an option (1 – 4):</h1>

Each option should function as follows:

<ul>

 <li>Option 1: Read in two imaginary numbers, add them together, and print out the result.</li>

 <li>Option 2: Read in two imaginary numbers, subtract the second one from the first, and print the result.</li>

 <li>Option 3: Read in two imaginary numbers, multiply them together, and print the result.</li>

 <li>Option 4: Print the message below and end the program</li>

</ul>

o    “Bye!”

Your program must use and implement the following functions:

<ul>

 <li>add: This function returns nothing and takes as parameters four floats (The real and imaginary parts of two imaginary numbers). The function also takes as parameters two float pointers (pointers to the imaginary and real portion of the result). This function adds the two imaginary numbers. This real part of the result is pointed to by the first pointer and the imaginary part of the result if pointed to by the second pointer. The function prototype is as follows:</li>

</ul>

o void add(float real_part_1, float imaginary_part_1, float real_part_2, float imaginary_part_2, float* real_result, float* imaginary_result)

<ul>

 <li>subtract: This function returns nothing and takes as parameters four floats (The real and imaginary parts of two imaginary numbers). The function also takes as parameters two float pointers (pointers to the imaginary and real portion of the result). This function subtracts the second imaginary number from the first. This real part of the result is pointed to by the first pointer and the imaginary part of the result is pointed to by the second pointer. The function prototype is as follows:</li>

</ul>

o void subtract(float real_part_1, float imaginary_part_1, float real_part_2, float imaginary_part_2, float* real_result, float* imaginary_result)

<ul>

 <li>multiply: This function returns nothing and takes as parameters four floats (The real and imaginary parts of two imaginary numbers). The function also takes as parameters two float pointers (pointers to the imaginary and real portion of the result). This function multiplies the two imaginary numbers. This real part of the result is pointed to by the first pointer and the imaginary part of the result if pointed to by the second pointer. The function prototype is as follows:</li>

</ul>

o void multiply(float real_part_1, float imaginary_part_1, float real_part_2, float imaginary_part_2, float* real_result, float* imaginary_result)

<ul>

 <li>read_num: This function returns nothing and takes as parameters two float pointers (The first pointer to the real part and the second pointer to the imaginary part of an imaginary number). This function begins by printing:</li>

</ul>

“Please type in the real component: ”

The function then reads in the real component of the imaginary number and points the first pointer passed to it to that number. Then the function prints:

“Please type the imaginary component: ”

The function then reads in the imaginary component of the imaginary number and points the second pointer passed to it to that number. The function prototype is as follows:

o void read_num(float *real_part, float *imaginary_part)

<ul>

 <li>read_nums: This function returns nothing and takes as parameters four float pointers (a pointer to the real part of the first imaginary number, a pointer to the imaginary part of the first imaginary number, a pointer to the real part of the second imaginary number, a pointer to the imaginary part of the second imaginary number). The function starts by printing: “Reading the first imaginary number…”</li>

</ul>

Then the function calls the read_num function to read in the first imaginary number. Then the function prints:

“Reading in the second imaginary number…”

The function then calls the read_num function to read in the second imaginary number. The function prototype is as follows:

o void read_nums(float* real_part_1, float* imaginary_part_1, float* real_part_2, float* imaginary_part_2)

<ul>

 <li>print_complex: This function returns nothing and takes as parameters two floats (one for the real part of the imaginary number and one for the imaginary part of the imaginary number). This function prints out the imaginary number by printing:</li>

</ul>

“The operation yields &lt;the real part of the number&gt; + &lt;the imaginary part of the number&gt;i” Both the imaginary and real parts of the number should be printed with 6 spaces and three numbers after the decimal point. The function prototype is as follows:

o void print_complex(float real_part, float imaginary_part)

Your program should function as follows (items underlined are to be entered by the user):

Complex Number Arithmetic Program:

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 4): <u>1</u>

<h1>Reading the first imaginary number…</h1>

<h1>Please type in the real component: <u>1.5</u></h1>

Please type in the imaginary component: <u>3.7</u>

Reading the second imaginary number…

Please type in the real component: <u>5.4</u>

Please type in the imaginary component: <u>2.3</u>

The operation yields  6.900 +  6.000i

<h1>1)     Add two complex numbers</h1>

<ul>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 4): <u>2</u>

Reading the first imaginary number…

Please type in the real component: <u>6</u>.

Please type in the imaginary component: <u>1.24</u>

Reading the second imaginary number…

Please type in the real component: <u>8.23</u>

Please type in the imaginary component: <u>6.754</u>

The operation yields -1.930 + -5.514i

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 4): <u>3</u>

Reading the first imaginary number…

Please type in the real component: <u>2.65</u>

Please type in the imaginary component: <u>3.7</u>

Reading the second imaginary number…

Please type in the real component: <u>5.4</u>

Please type in the imaginary component: <u>2.31</u>

The operation yields  5.763 + 26.102i

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 4): <u>5</u>

Please input a valid menu option

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 4): <u>4</u> Bye!

<strong>Notes: </strong>

<ul>

 <li>If the user enters an invalid menu option, the program should print the following error message:</li>

</ul>

“Please input a valid menu option”

<ul>

 <li>For each operation (add, subtract, multiply) you can assume the user will give valid input</li>

</ul>




Save your program as complex_calculator.c




<strong>Challenge for problem 1 </strong>(10 extra credit points):

Add a division operation to your calculator. The menu is as follows:

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Divide two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 5):

Each option must function as follows:

<ul>

 <li>Option 1-3: The same as before</li>

 <li>Option 4: Read in two imaginary numbers, divide the first by the second, and print the result.</li>

 <li>Option 5: Print the message below and end the program</li>

</ul>

&#x25aa;    “Bye!”

Your program can use the previous functions and add the following function:

<ul>

 <li>divide: This function returns nothing and takes as parameters four floats (The real and imaginary parts of two imaginary numbers). The function also takes as parameters two float pointers (pointers to the imaginary and real portion of the result). This function divides the first imaginary number by the second. This real part of the result is pointed to by the first pointer and the imaginary part of the result is pointed to by the second pointer. The function prototype is as follows:</li>

</ul>

o void divide(float real_part_1, float imaginary_part_1, float real_part_2, float imaginary_part_2, float* real_result, float* imaginary_result) Your program should function as follows (items underlined are to be entered by the user):

Complex Number Arithmetic Program:

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Divide two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 5): <u>4</u>

Reading the first imaginary number…

Please type in the real component: <u>2</u> Please type in the imaginary component: <u>-1</u>

Reading the second imaginary number… Please type in the real component: <u>-3</u>

Please type in the imaginary component: <u>6</u>

The operation yields -0.267 + -0.200i

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Divide two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 5): <u>6</u>

Please input a valid menu option

<ul>

 <li>Add two complex numbers</li>

 <li>Subtract two complex numbers</li>

 <li>Multiply two complex numbers</li>

 <li>Divide two complex numbers</li>

 <li>Quit</li>

</ul>

Choose an option (1 – 5): <u>5</u> Bye!

Save your challenge separately as complex_calculator_c.c





