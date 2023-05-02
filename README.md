Download Link: https://assignmentchef.com/product/solved-comp1020-lab1-input-output-if-and-loops
<br>
Introduction to basic Java

Notes:

<ul>

 <li>These exercises are intended to give you basic practice in using Java (as opposed to Processing or Python).</li>

 <li>You should definitely do at least the Bronze and Silver exercises. You can do these o before the lab, on your own, using any Java programming environment you like, or o during the lab, using DrJava, with assistance from the lab TA, or o after the lab, on your own.</li>

 <li>For credit, you must demonstrate at least one working exercise, in the lab, using DrJava.</li>

 <li>Make sure your TA has recorded your mark before leaving.</li>

 <li>The three questions are sequential – each builds on the previous one.</li>

 <li>Each exercise should require roughly 15 lines of actual code (in addition to the code from the previous exercises). This does not include blank lines, } lines, or comments.</li>

 <li>Always try to complete as many exercises as you can on every lab. For Lab 1, everyone should try to complete at least the Bronze and Silver exercises.</li>

</ul>




<ol>

 <li>Download the file <strong>java</strong> from the course website.</li>

 <li>Complete the <strong>readData( )</strong> method so that it operates as follows:

  <ol>

   <li>It should repeatedly prompt the user to enter an integer value, and then react as follows:

    <ol>

     <li>Values between 1 and 100 are “valid”. It should print out a message which echoes the value, and indicates that it is valid, as shown below. It should also keep track of the number of such valid values that were entered.</li>

     <li>The value 0 is special, and should cause the method to quit. Nothing should be printed out in this case.</li>

    </ol></li>

  </ol></li>

</ol>

<ul>

 <li>All other values should print an error message, as shown below.</li>

</ul>

<ol>

 <li>It should return the number of valid values that were entered.</li>

</ol>

<ol start="3">

 <li>The output from the program should look like this. Note that the last line is printed by the supplied main method, not by your code. User input is shown in red.</li>

</ol>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>50</strong>

<strong>Entry 50 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>99</strong>

<strong>Entry 99 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>123</strong>

<strong>Invalid entry rejected. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>-42</strong>

<strong>Invalid entry rejected. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>1</strong>

<strong>Entry 1 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>0</strong><strong> 3 valid entries were read in. </strong>

<ol>

 <li>Modify your program as follows:

  <ol>

   <li>Add a parameter of type <strong>int[]</strong> (array of integers) to the existing <strong>readData</strong> The method should now store all of the valid values (but not the 0 or the invalid ones) into this array.</li>

   <li>Write a method <strong>void printArray(int[] a, int n)</strong> which will print out the first <strong>n</strong> elements in the array <strong><sub>a</sub></strong>, in the format shown in the example below. The numbers should be separated by commas, but there should be no comma after the last one. There should be no blanks.</li>

   <li>Write a method <strong>double average(int[] a, int n)</strong> which will find and return the average of the first <strong><sub>n</sub></strong> values in the array <strong><sub>a</sub></strong>. Be careful to return an accurate value calculated as a <strong><sub>double</sub></strong>, not as an <strong><sub>int</sub></strong>. In the example below, the average should be 54.3333 not 54.0.</li>

   <li>Modify the <strong><sub>main</sub></strong> method so that it creates an array capable of holding up to 100 <strong><sub>int</sub></strong> Use the <strong><sub>readData</sub></strong> method to place the input values into this array. Then use the <strong>printArray</strong> and <strong>average</strong> methods to print the elements from the array, and their average, as shown below.</li>

  </ol></li>

 <li>The output from the program should now look like this:</li>

</ol>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>50</strong>

<strong>Entry 50 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>99</strong>

<strong>Entry 99 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>203</strong>

<strong>Invalid entry rejected. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>14</strong>

<strong>Entry 14 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>0</strong>

<strong>3 valid entries were read in: </strong>

<strong>50,99,14 </strong>

<strong>Their average is 54.333333333333336 </strong>

<strong> </strong>




Make the following further modifications to the program:

<ol>

 <li>Modify the <strong><sub>readData</sub></strong> method so that it keeps the values in the array <strong><em>sorted</em></strong> into ascending order at all times. Each new value must be placed in the proper position, with all larger values shifted up by one position.</li>

 <li>Write a method <strong>double median(int[] a, int n)</strong> which will find the median of the first <strong>n</strong> elements of the array <strong><sub>a</sub></strong>. As long as the array is in ascending order (which it should be), the median is defined as follows: if <strong><sub>n</sub></strong> is odd, then the median is the middle value, and if <strong><sub>n</sub></strong> is even the median is the average of the two middle values. For example, the median of 1,4,19,45,199 is 19 and the median of 1,4,19,22,45,99 is 20.5 (the average of 19 and 22). <em>Try to write this method in one line, without using an if statement. Think about it.</em></li>

 <li>Modify the main program so that it prints the median as well as the average.</li>

 <li>The output of the program should now look like this:</li>

</ol>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>45</strong>

<strong>Entry 45 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>19</strong>

<strong>Entry 19 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>99</strong>

<strong>Entry 99 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>4</strong>

<strong>Entry 4 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>1</strong>

<strong>Entry 1 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>22</strong>

<strong>Entry 22 accepted. </strong>

<strong>Enter an integer from 1 to 100 (0 to quit):</strong><strong>0</strong>

<strong>6 valid entries were read in: </strong>

<strong>1,4,19,22,45,99 </strong>

<strong>Their average is 31.666666666666668 </strong>

<strong>Their median is 20.5 </strong>


