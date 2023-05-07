Download Link: https://assignmentchef.com/product/solved-lab-exercise-8-problems
<br>
<ol>

 <li>Write C++ programs</li>

 <li>Compile C++ programs</li>

 <li>Implement programs that use recursion to solve advanced problems</li>

</ol>

<h1><a id="user-content-additional-reading" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08#additional-reading" aria-hidden="true"></a>Additional Reading</h1>

This lab exercise requires an understanding of some concepts to solve the problems. You are strongly encouraged to read the following tutorials to help you answer the problems.

<ol>

 <li><a href="https://github.com/ILXL-guides/function-file-organization">Organizing C++ files: function prototypes, implementations, and drivers</a>.</li>

 <li><a href="https://github.com/ILXL-guides/object-parameters-and-return-values">Using objects as parameters and return values in functions</a></li>

 <li><a href="https://github.com/ILXL-guides/arrays-as-parameters">Passing arrays as parameters to functions</a></li>

 <li><a href="https://github.com/ILXL-guides/cpp-file-io">File reading and writing (also includes dealing with arrays)</a></li>

</ol>

<h1><a id="user-content-instructions" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08#instructions" aria-hidden="true"></a>Instructions</h1>

Answer the programming problems sequentially (i.e., answer prob01 before prob02). If you have questions let your instructor or the lab assistant know. You can also consult your classmates.

When you answer two programming problems correctly, let your instructor know and wait for further instruction.

<h1><a id="user-content-lab-exercise-guide" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08#lab-exercise-guide" aria-hidden="true"></a>Lab exercise guide</h1>

Here’s a link to the <a href="https://docs.google.com/document/d/1EX01EtrO-pkHNLVPxiq7HNh1f5KnJZnr_dlJcO4T7t0/edit?usp=sharing" rel="nofollow">Lab exercise guide</a> in case you need to review the lab exercise objectives, grading scheme, or evaluation process.

<h1>Count Odd</h1>

Create a program that counts all the odd numbers from 0 to a number using recursion. Your program should have a function called <code>count_odd</code> that takes in an <code>int</code> value and returns an <code>int</code> value. The user will be asked for a number, and the program will display the following output.

<h2><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob01#sample-output" aria-hidden="true"></a>Sample Output:</h2>

<pre>Enter a number: <b>5</b>The number of odds from 0 to 5 is 3</pre>

<pre>Enter a number: <b>13</b>The number of odds from 0 to 13 is 7</pre>

Place the <code>count_odd</code>‘s function prototype in <code>count-odd.hpp</code> and it’s implementation in <code>count-odd.cpp</code>. The <code>main</code> function already contains some code, but you need to complete the requirements that is described inside the file.

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob01#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob01#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>count-odd.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp count-odd.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Linear Search Array</h1>

Create a recursive <code>linear_search</code> function that receives an integer array (<code>int[]</code>), a number to find in the array, and the size of the array. The function should return the index of the number in the array if it exists, and returns -1 if it isn’t in the array.

Place the <code>linear_search</code>‘s function prototype in <code>lsa.hpp</code> and it’s implementation in <code>lsa.cpp</code>. The <code>main</code> function already contains some code, but you need to complete the requirements that is described inside the file.

<h1><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob02#sample-output" aria-hidden="true"></a>Sample output:</h1>

<pre>Array: 3 16 22 8 11 0 55 34 27 31Please enter a number you want to search for: <b>8</b>The index of 8 in the array is: 3</pre>

<pre>Array: 3 16 22 8 11 0 55 34 27 31Please enter a number you want to search for: <b>15</b>15 is not in the array</pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob02#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob02#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>lsa.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp lsa.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Recursive Power Function</h1>

Create a recursive function called <code>power</code> that receives two <strong>positive</strong> <code>int</code> parameters that represent the base and exponent. The function should return the base raised to the exponent.

Place the <code>power</code>‘s function prototype in <code>power.hpp</code> and it’s implementation in <code>power.cpp</code>. The <code>main</code> function already contains some code, but you need to complete the requirements that is described inside the file.

<h1><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob03#sample-output" aria-hidden="true"></a>Sample Output:</h1>

<pre>Enter a base: <b>5</b>Enter an exponent: <b>3</b>5 ^ 3 = 125</pre>

<pre>Enter a base: <b>2</b>Enter an exponent: <b>10</b>2 ^ 10 = 1024</pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob03#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob03#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>power.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp power.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>GCD calculator</h1>

Create a recursive Greatest Common Divisor (GCD) calculator function called <code>gcd</code> that receives two integer inputs. The function should return the GCD of those two numbers.

There are two methods to compute the GCD of two numbers: <em>Euclidean</em> and <em>Dijkstra’s</em> algorithm. You can choose either of the two algorithms to implement your recursive <code>gcd</code> function.

<h2><a id="user-content-euclidean-algorithm" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob04#euclidean-algorithm" aria-hidden="true"></a>Euclidean Algorithm</h2>

The Euclidean algorithm mainly uses division and the remainder of the two numbers to find the GCD. It can be represented as a recursive algorithm such that

<pre><code>gcd(num1, num2) = num2                      if num1 == zero // base case                = gcd(num2 % num1, num1)    if num1 &gt; zero  // recursive case</code></pre>

You can learn more about this topic by going through these <a href="https://docs.google.com/presentation/d/11NvpHUof67flvwiDCzcMR4fMhZ2x56EOgDgrTa_dZ9M/edit?usp=sharing" rel="nofollow">slides</a>.

<h2><a id="user-content-dijkstras-gcd-algorithm" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob04#dijkstras-gcd-algorithm" aria-hidden="true"></a>Dijkstra’s GCD algorithm</h2>

Dijkstra’s algorithm mainly uses subtraction to find the GCD. It can be represented as a recursive algorithm such that

<pre><code> gcd(num1, num2) = num2                     // if num1 and num2 are equal                 = gcd(num1 - num2, num2)   // if num1 is greater than num2                 = gcd(num1, num2 - num1)   // if num2 is greater than num1</code></pre>

As an example, lets say we want to find the GCD of the two numbers 72 and 56

<pre><code>gcd(72 , 56)  72-56 , 56  Take the larger number, 72 and subtract 56 from it  16 , 56     This is our end result, but we need to keep going. Until they are equalgcd(16 , 56)  16 , 56-16  Take the larger number,56 and subtract 16 from it  16 , 40     This is our end result, but this still doesnt give us our gcd, so we keep going until both numbers are equalgcd(16 , 40)  16 , 40-16  Take the larger number 40 and subtract 16 from it.  16 , 24     This is our end result, but this still doesnt give us our gcd, so we keep going until both numbers are equalgcd(16,24)     16 , 24-16  Take the larger number 24 and subtract 16 from it.  16 , 8      This is our end result, but this still doesnt give us our gcd, so we keep going until both numbers are equalgcd(16, 8)     16-8, 8     Take the larger number 16 and subtract 8 from it.  8 ,8        this is our end result, and on the next function call we will validate the equality of those two numbers there.gcd(8,8)  8 , 8       The two numbers are equal. THIS IS OUR GCD.</code></pre>

You can learn more about this topic by going through these <a href="https://docs.google.com/presentation/d/1EulZVpBq6cJmv_VSjzcpLW15FBCfacun6J9PMrxNRwE/edit?usp=sharing" rel="nofollow">slides</a>

Place the <code>gcd</code>‘s function prototype in <code>gcd.hpp</code> and it’s implementation in <code>gcd.cpp</code>. The <code>main</code> function already contains some code, but you need to complete the requirements that is described inside the file.

<h2><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob04#sample-output" aria-hidden="true"></a>Sample Output</h2>

<pre>Enter the first number: <b>24</b>Enter the second number: <b>18</b>The GCD of the numbers 24 and 18 is 6</pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob04#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob04#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>gcd.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp gcd.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Max Value</h1>

Write a program that finds the largest number in an array of positive numbers using recursion. Your program should have a function called <code>array_max</code> that should pass in an <code>int</code> array, and an <code>int</code> for the size of the array, respectively, and should return an <code>int</code> value.

Given an array of size 10 with contents: <code>{10, 9, 6, 1, 2, 4, 16, 8, 7, 5}</code>

The output should be:

<pre><code>The largest number in the array is 16</code></pre>

<em>The function should return -1 if the input is invalid.</em>

Place the <code>array_max</code>‘s function prototype in <code>array_max.hpp</code> and it’s implementation in <code>array_max.cpp</code>. The <code>main</code> function already contains some code, but you need to complete the requirements that is described inside the file.

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob05#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_08/prob05#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>array_max.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp array_max.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>


