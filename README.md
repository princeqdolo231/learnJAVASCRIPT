<div align="center">
  <h1>JAVASCRIPTS CRASH COURSE REVEIW</h1>
</div>
<ul>
  <li><a href="https://github.com/princeqdolo231/learnJAVASCRIPT/blob/main/AssignmentOne.md" ></a>JavaScript Function</li>
</ul>
<br>

<h1>What is JavaScript ?</h1>

<p>
  JavaScript is a high level, interpreted programing language that conforms to the ECMAScript specification.
  It also a programming language with Multi-Paradigm which is you can write your JavaScript in many ways, eithier by object oriented or functional.
  Lastly, Javascript is a programming language that run on both the browser and sever.
</p>
<p>
  Here are few important topics to look at in <i>JavaScript</i>
</p>

<ol>
  <li>Variables and Data Types</li>
  <li>Arrays</li>
  <li>Objects Literals</l>
  <li>Methods for strings, arrays, objects, etc</li>
  <li>Loops - for, while, for...of, forEach, map</li>
  <li>Conditionals (if, ternary & switch)</li>
  <li>Functions (normal & arrow)</li>
  <li>OOP (prototypes & classes)</li>
  <li>DOM selection</li>
  <li>DOM Manipulation</li>
  <li>Events</li>
  <li>Basic form validation</li>
</ol>

<h3> 1. Variables and Data Types</h3>
<p>
  Javascript variables is a containers used to stored data, in JavaScript their are three ways or mether we used to store variables.
</p>
<ol>
  <li>We use the **var** key word to stored data.</li>
  <li>We use the **let** key word to stored data.</li>
  <li>And we also use the **const** key word to stored data as well.</li>
</ol>
<p>
  As for JavaScript **Data Types** we have **8** types of data types but we will only discuss 3 here.
  These four types are: <b>String</b>, <b>Numbers</b>, and <b>Boolean</b>.
</p>

<pre>
  <code>
    // Numbers:
    let length = 16;
    let weight = 7.5;

    // Strings:
    let color = "Yellow";
    let lastName = "Johnson";

    // Booleans
    let x = true;
    let y = false;
  </code>
</pre>


<h3>2. Arrays</h3>
What is a array ?
An array is a special variable, which can hold more than one value: <br>
Example:
<pre>
  <code>
        const cars = ["Saab", "Volvo", "BMW"];
  </code>
</pre>



<h3>3. Objects Literals</h3>

0bject literals are one of the most commonly used data structures in JavaScript. They are used to store collections of data, and can be used to represent complex data structures such as objects, arrays, functions, and even regular expressions. Object literals are also used to store information about a particular instance of an object, such as its state or behavior.

Object literals are written in the form of key-value pairs, where each key is a string and each value can be any valid JavaScript data type. For example, the following object literal stores information about a person: <br>

<pre>
  <code>
    const person = {
      name: 'John Doe',
      age: 30,
      address: '123 Main Street'
    };
  </code>
</pre>

Object literals can also contain other object literals, as well as functions. For example, the following object literal stores information about a person, and also contains a function that prints out a greeting message:
<pre>
  <code>
    const person = {
      name: 'John Doe',
      age: 30,
      address: '123 Main Street',
      greet: function() {
    
    console.log('Hello, my name is ' + this.name);
  }
  </code>
</pre>

<h3>4. Methods for strings, arrays, objects, etc.</h3>

<ul>
  <li><b>Strings Method</b></li>
</ul>
<p>
  Strings are used to hold data that can be represented in text form. To create a string you can use the String() constructor or a string literal. 
</p>
<pre>
  <code>
    // Using a constructor:
    let string1 = String ('String Creation')
  </code>
  
  <code>
    // Using a string literal:
    let string2 = 'String Creation');
  </code>
</pre>

<b>The .charAt() method</b>
<p>
  A lot of the time when working with strings, we want to access a character at a certain index of the string. You can do this either with the       
  charAt() method or with indexing, the same way we treat an array.
</p>

<pre>
  <code>
    // Let's say we want to access the first character of a given string
 let string = 'Hello World';
 
    // using indexing
 let first1 = string[0]; 
    // output 'H' and remember that indexing starts at 0
 
   // using the charAt() method
 let first2 = string.charAt(0); 
    // output 'H'
  </code>
</pre>

<b>The .toUpperCase() and .toLowerCase() methods</b>
<p>
  Now let's say we want to uppercase or lowercase a string. You can do this using the toUpperCase() and the toLowerCase() instance methods.
</p>

<pre>
  <code>
    let string = 'Hello';
 
  // Let's lowercase a string
 
 let lowerCase = string.toLowerCase(); 
    // output 'hello'
 
  // Let's upperCase a string
  
 let upperCase = string.toUpperCase(); 
    // output 'HELLO'
  </code>
</pre>

<ul>
  <li><b>Array Method</b></li>
</ul>
<p>
  Like other programming languages, JavaScript arrays let you store a collection of data under one variable. But unlike C or C++, arrays can be   
  returned from function calls.

  JavaScript arrays are dynamic, so you can add to or delete elements from an array. You can also have elements of multiple data types in a single 
  array.

  Let's talk about how to create arrays in JavaScript. You can easily create an array by assigning a variable to empty brackets [ ] or by using the   
  Array() constructor.
</p>

<pre>
  <code>
    // Creating an array from constructor
 
    let arr1 = Array();
 
   // Prefered method
 
    let arr2 = [];
  </code>
</pre>
<p>
  Now let's look at some important array instance and class methods that I consider to be the most useful.
</p>

<b>The .indexOf() method</b>
<p>
  Now let's say we want to uppercase or lowercase a string. You can do this using the toUpperCase() and the toLowerCase() instance methods.
</p>

<pre>
  <code>
   let array = [1, 2, 3];

 // Let's find the index where 1 occurs for thwe first time
 
  let first1 = array.indexOf(1); 
    // output 0

 // Now let's try to find 4 in the array
 
let first4 = array.indexOf(4); 
    // output -1
  </code>
</pre>

<b>The .push() and .pop() methods</b>
<p>
  As I mentioned earlier, JavaScript arrays are dynamic. So we can add elements using the push() method and remove the last element using the pop() 
  method. An important note is that both of those methods mutate the original array.
</p>

<pre>
  <code>
   let array = [1, 2, 3];

 // let's add 4 to the array
 
array.push(4)

console.log(array) 
    // output [1, 2, 3, 4]

 // let's now make the array the same as before
 
let removedElement = array.pop() 
    // output 4

console.log(array) 
    // output [1, 2, 3]
  </code>
</pre>

<h3>5. Loops - for, while, for...of, forEach, map</h3>

<ul>
  <li><b>For Loop</b></li>
</ul>

<p>
  The for statement creates a loop with 3 optional expressions:
</p>
<pre>
  <code>
    for (expression 1; expression 2; expression 3) {
  // code block to be executed
}
  </code>
</pre>
<p>
  <b>Expression 1</b> is executed (one time) before the execution of the code block.
  <br>
  <b>Expression 2</b> defines the condition for executing the code block.
  <br>
  <b>Expression 3</b> is executed (every time) after the code block has been executed.
</p>
<p>Example:</p>
<pre>
  <code>
    for (let i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
    // The results will be:
        The number is 0
        The number is 1
        The number is 2
        The number is 3
        The number is 4
}
  </code>
</pre>

<ul>
  <li><b>While</b></li>
</ul>
<p>
  The while loop loops through a block of code as long as a specified condition is true.
</p>
<pre>
  <code>
    while (condition) {
  // code block to be executed
}
  </code>
</pre>
<p>
  Example:
</p>
<p>
  In the following example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10:
</p>
<pre>
  <code>
    while (i < 10) {
  text += "The number is " + i;
  i++;
}
  // The results will be:
        The number is 0
        The number is 1
        The number is 2
        The number is 3
        The number is 4
        The number is 5
        The number is 6
        The number is 7
        The number is 8
        The number is 9
  </code>
</pre>


<ul>
  <li><b>For...of</b></li>
</ul>
<p>
  The JavaScript <b><em>for...in</em></b> statement loops through the properties of an Object:
</p>
<pre>
  <code>
    for (key in object) {
  // code block to be executed
}
  </code>
</pre>
<p>
  Example:
</p>
<pre>
  <code>
    const person = {fname:"John", lname:"Doe", age:25};
       let text = "";
       for (let x in person) {
       text += person[x];
   }
      // The results will be:
      The for in statement loops through the properties of an object:
      John Doe 25
  </code>
</pre>

<ul>
  <li><b>forEach</b></li>
</ul>
<p>
  The <b><em>forEach()</em></b> method calls a function for each element in an array.
</p>
<p>
  The <b><em>forEach()</em></b> method is not executed for empty elements.
</p>
<pre>
  <code>
    const fruits = ["apple", "orange", "cherry"];
      fruits.forEach(myFunction);
    // The result will be:
      0: apple
      1: orange
      2: cherry
  </code>
</pre>


<ul>
  <li><b>map</b></li>
</ul>

<h3>6. Conditionals (if, ternary & switch)</h3>

<ul>
  <li><b>ternary statemrnts:</b></li>
</ul>

<ul>
  <li><b>switch statemrnts:</b></li>
</ul>
