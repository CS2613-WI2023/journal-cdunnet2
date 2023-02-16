# Cody's Journal

## JavaScript Block

### Syntax & Semantics 

#### Syntax Basics

A lot of the syntax is similar to, unsuprisingly, Java. Things like **for loop structure**:
```
for(var x = 0; x < y; x++){
```
or just function structure in general tend to show similarity. We have `const` for constants, and we define objects in a similar way, `horse = new Horse()`. We still use semicolons to end a line, and in general JavaScript *can* look like many other programming languages.

#### JavaScript Uniqueness

Some things that stood out to me were things like **nested functions**, **arrow functions**, or **function callbacks**. Nested functions are interesting, because typically each function would be in its own block. JavaScript functions are different than many other programming language 'methods' as they can be defined pretty much anywhere. For example:
```
function calculate() {
    const number1 = 1;
    const number2 = 2;

    function subtract() {
        return number1 - number2;
    }
    return subtract()
}
```
Personally I like the idea of each "function" a program needs to perform being in its own block, but allowing this sort of nesting opens up different possibilities, and allows for different use of scope for specific variables.

Arrow functions are one of the more interesting aspects, and represent a more compact way of formatting functions that don't need some of the more in-depth accompanying keywords like `super`, `this`, `yield`, and [some others](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions). An example of arrow functions in Q2 would be:

```
setTimeout(() => {
          callback(names[index]);
          resolve();
        }, timeoutTime);
```
As demonstrated, arrow function allows for a sort of combination parameter in the setTimeout() function.


Finally, the addition of *function callbacks*, as used in Q2 are a neat way of getting specific information from a function, without explicitly defining what it should be. First, we take a callback as a parameter:
```
async function haircut(times, names, callback) {
```
Then, we define what we want the callback to be:
```
callback(names[index]);
```

We define the callback function within the parameters, in this case we use a new variable called `(name)`, which we show within parentheses before the function - in this case the function was a simple console.log() that used `name` inside:
```
haircut(durations, names, (name) => {
```

I believe each of these ways of using JavaScript can be extremely helpful and ultimately make up some of the fundemental reasons why the language is used.


### Supported Paradigms

JavaScript seems to be mostly used for web development in tandem with HTML & CSS. In their documentation on web scripting, [Mozilla explains that](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript) HTML defines a structure for a webpage, CSS controls how elements look on a webpage, and JavaScript does, *"pretty much everything else"*.

#### My Own Experience 

In my workplace, we use JavaScript in a couple of forms. One is the general use, in client-side scripting on an internal company-only webpage. We use JavaScript to keep track of things like employee number and any other type of relevent information for a given page, which gives us access to this information without the employee explicitly writing it down. We then can display it on the page or use it in functions.

The second way we use JavaScript is within our webpage driver code. It is sort of used in the same way, where we use existing variables within the JavaScript function, but we store the function code within a string and pass the whole function code as a variable when needed. I believe this application is used for things like email structure for an auto-generated email, and sometimes to be sent to a given server machine to be run on it instead of the client.

### Data Structures and Libraries

#### Libraries
There are *many* different JavaScript libraries with some of the most popular being jQuery and React. I knew of them but was unfamiliar with their use, and it seems that jQuery adds many functions that make JavaScript a more accessible tool. On their [main site](https://jquery.com), they demonstrate the addition of button on-click handling, and API calls for local weather. This shows the sheer variety in things you can accomplish using jQuery - even just by connecting to certain APIs.

#### Data Structures 

JavaScript supports many of the usual data types like arrays, and they can be defined without specifying the data type housed within. As for other more complex structures, lists, queues, trees, etc. are all possible. In fact, you can even make trees using [nested arrays](https://medium.com/@mahendrjy/javascript-trees-b8f3b4261c3a), though this is probably best kept for small, non-scaling use cases.

Because JavaScript is object-oriented, data structures can work pretty much the same as other OOP languages, with any required 'node' as a defined object.

### Under-the-hood

[As previously mentioned](#supported-paradigms), JavaScript is a scripting language mainly used for web development. As such, it is not really supposed to be used alone, and is much more of a team player. Though the number seems to be different depending on the source, JavaScript is consistently claimed to be in over 90% of websites, and is often surveyed to be one of the most commonly used [programming](https://insights.stackoverflow.com/survey/2019#technology) [languages](https://survey.stackoverflow.co/2022/#technology). 

JavaScript does a lot for you and is definitely a high level language - you won't be stuck using pointers or `malloc` like you would in C.


## Racket Block

### Syntax & Semantics 

### Supported Paradigms

### Data Structures and Libraries

### Under-the-hood



## Matlab/Octave Block

### Syntax & Semantics 

### Supported Paradigms

### Data Structures and Libraries

### Under-the-hood


