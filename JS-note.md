### \#What Is a Data Type, and What Are the Different Data Types in JavaScript?

#### 

#### 1-data type

a data type is the kind of value you store like a number or piece of text.



A variable is a named container that stores a value of a specific data type, allowing you to reference and manipulate it throughout your code.

&#x20;



##### \*Number:

A Number represents both integers and floating-point values. Examples of integers include 7, 19, and 90.









#### \*String:

A String is a sequence of characters, or text, enclosed in quotes.

Here is an example string using double quotes: console.log("I love to code!");



+++In JavaScript, a string is a sequence of characters used to represent text data. Strings are one of the primitive data types in the language, along with numbers, booleans, null, and undefined.



To create a string in JavaScript, you can use single quotes ('), or double quotes (").

+++





Here is an example of creating two variables that hold string values:



let singleQuotes = 'This is a string';

console.log(singleQuotes);

let doubleQuotes = "This is also a string";

console.log(doubleQuotes);



+++++

















Another thing to take into account is that strings are immutable. In programming, immutability means that once something is created, it cannot be changed. So, when you create a string, you can't change its characters directly. Instead, you would create a new string if you want to make changes.

















+++++



Here is an example of assigning a new string to a developer variable:



let developer = "Jessica";

console.log(developer);

developer = "Quincy";

console.log(developer);

Since strings are immutable, we can't update the first string directly. That is why we are assigning a new string to the developer variable.



+++++











#### \*Boolean

A Boolean represents one of two values: true or false. For example, a program might check whether a user is logged in (true) or not (false) and change the page based on that. If the user is logged in, you probably want to show them the dashboard page. Otherwise, you will want to show them the login page.









##### \*undefined

means a variable has been declared but hasn't been given a value yet.









##### \*null

means the variable has been intentionally set to "nothing" and does not hold any value.







### 

### 2-Object

Objects are great for grouping related information together.

An Object is a collection of key-value pairs.



{

&#x20; name: "Alice",

&#x20; age: 30

};









### 3-Symbol

A Symbol is a special type of value in JavaScript that is always unique and cannot be changed. It's often used to create unique labels or identifiers for properties:



Symbol('mySymbol');











#### 4-BigInt

BigInt is used for very large numbers that exceed the limit of the Number type:

1234567890123456789012345678901234567890n;

In this example, we create a BigInt by adding n at the end of a very large number.









## \#What Are Variables, and What Are Guidelines for Naming JavaScript Variables?







#### 5-variables



In JavaScript, variables act as containers for storing data that you can access and modify throughout your program.



You can think of variables as boxes that hold values. With variables, you can keep track of things like numbers or text and refer to these values whenever you need them in your program.









##### \*let

One way to declare a variable in JavaScript is to use the let keyword. You will learn more about the let keyword as well as other ways to declare variables in future lessons.



Here's an example of using let to declare a variable called age:



let age;



+++

Right now, the age variable does not have a value assigned to it. If you try to use it, it will return undefined, which means it has no value.

+++



let age;

console.log(age); // undefined

To assign a value to a variable you will need to use the assignment operator like this:



let age = 25;

Now when you use the age variable, it will return the value of 25.



let age = 25;

console.log(age); // 25



++++++++++++++++++++++++++++++++++++++++++++++++++ Variables in JavaScript must begin with a letter, an underscore (\_), or a dollar sign ($). They cannot start with a number.



// Valid variable names

let age;

let \_score;

let $total;



// Invalid variable names

let 1stPlace; // starts with a number



+++++++++++++++++Variable names are case-sensitive, meaning the word age in all lowercase and the word Age with a capital A are considered different variables.



let age = 25;

let Age = 30;

console.log(age); // 25

console.log(Age); // 30

This is why it's important to stick with a consistent naming convention like camelCase. camelCase is where the first word is all lowercase and each subsequent word starts with an uppercase letter.



You should also avoid using special characters like exclamation points (!) or at (@) symbols, in your variable names. It is best to keep variable names readable by using letters, numbers, underscores, or dollar signs.















#### 6-let

The let keyword allows you to declare variables that can be updated or reassigned later. You can think of let as a flexible container – once you've stored a value in it, you can change that value as needed throughout your program.



+++++Here's an example of declaring and assigning a variable with let:



let score = 10;

In this case, the variable score is declared and assigned the value 10. If you want to update the value later, you can easily do that:



let score = 10;

console.log(score); // 10

score = 20;

console.log(score); // 20



+++++++

You can declare a let variable without immediately assigning it a value, and you can assign it a value later

+++++++











#### 7-const

This makes const ideal for values that you don't want to change accidentally during the execution of your program.



Here's an example of declaring and assigning a variable with const:



const maxScore = 100;

console.log(maxScore); // 100





+++Trying to reassign a value to a const variable will throw an error in your JavaScript console, as const variables are immutable once they are assigned.



+++Variables declared with const must be assigned a value at the time of declaration. If you try to declare a const variable without assigning it a value, you will get an error

