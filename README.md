Download Link: https://assignmentchef.com/product/solved-csci321-project-five-a-random-string-generator
<br>
<strong>Objectives:</strong>

<ol>

 <li>Write user defined procedures</li>

 <li>Call and test user defined procedures</li>

 <li>Use Irvine.inc library to take input and display output.</li>

</ol>

<strong>Problem Description:</strong>

Create a procedure that generates a random string of Length L, containing all capital letters. When calling the procedure, pass the value of L in EAX, and pass a pointer to an array of byte that will hold the random string. Write a test program that calls your procedure 20 times and displays the strings in the console window. In your program, the random string size shall be preset as a constant.

<strong>How to See Result</strong>

You may notice that your console window will show up then quickly disappear. You have two ways to view your result from console window. One way is to set the break point at exit statement in main procedure. Another way is to add the following statement before exit statement in main procedure:

<em>Call ReadChar</em>

This will hold the console window to wait for your input. You can hit any key to close the console window. It is better if you add a prompt to tell user what to do. For instance: “Press any key to continue…”. To do so, you simply add

prompt BYTE “Press any key to continue…”, 0

in your .data section and add the following code before Call ReadChar:

<em>move dx, OFFSET prompt</em>

<em>Call WriteString</em>

<strong>Sample Run:</strong>