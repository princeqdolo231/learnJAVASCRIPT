<h1>FUNCTIONS</h1>
JavaScript functions are reusable blocks of code that perform a specific task, taking some form of input and returning an output.

To define a function, you must use the function keyword, followed by a name, followed by parentheses ( ). Then you have to write the function logic between curly brackets { }

Here is an example of how to write a function in JavaScript:
<pre>
  <code>
    EXAMPLE:
    
    function addTwoNumbers(x, y) {
           return x + y;
    }
  </code>
</pre>

<strong>There’s a lot going on in the example above, so let’s look at each part individually.</strong>

<strong>“Function”</strong> is the keyword required to actually start declaring a function
“addTwoNumbers” is the function’s name, which is customizable. Function names can contain letters, numbers, and certain special characters, just like variables.
(x, y) are parameters, which are variable names for the inputs the function will accept. These parameters are also referred to as arguments.
“Return” is the keyword that exits the function and shares an optional value outside
The code that the function will execute must be put inside of curly brackets { }

<h1>Using functions</h1>
Once a JS function is defined (declared), you can use it by referencing its name with parentheses ( ) right after. Note that a function doesn’t have to have parameters - they can simply be left blank in the parentheses:

<pre>
  <code>
    EXAMPLE:
    
    function greetThePlanet() {
           return "Hello world!";
    }
​
          greetThePlanet();
          OUTPUT
          "Hello world!"
  </code>
</pre>

There can be zero, one, or multiple arguments in a function.<br> 
In the example above, the function "greetThePlanet" simply returns the phrase "Hello World!", and it doesn't require any parameters (arguments) in order to do so.

However, if a function does have parameters, you’ll need to provide values inside the parentheses when using the function:

<pre>
  <code>
    EXAMPLE
     function square(number) {
       return number * number;
}
​
        square(16);
        OUTPUT
        256
  </code>
</pre>

In the example above, you have to provide a number inside of the parentheses in order for the function to work and to receive a proper output. Otherwise, your code won’t work and you’ll get an error message.

If your function takes more than one argument, simply separate them with a comma inside of the parentheses. <br>
You can refer to the "addTwoNumbers" function at the top of this page for an example.
