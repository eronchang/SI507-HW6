# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* Like this:
* **Ting-Wei Chang (changtw)**
* Shaoxian Lin (elainlin)
* Meng Wang (mwscott)


## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

A code comment would require 2 "/" before your comment text, something like

```js
//my comment
```

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

You will need a browser, like Chrome or Firefox to open it. Or, you can also use a Flask application to render ".html" files as we did in the previous assignments as templates.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

There are two:
<br> 1.```js
alert()
```
This function can only result contents to show up in document for normal users.
<br> 2.```js
console.log()
```
This function would result content to be shown only in console, which could be a function you would use if you only want to show contents for programmers.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

You would have to comment out the line of
```js
alert("hello") //add "//" before this line
```
on line 12 and add
```js
alert(Date());
```


* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

You change in the line
```js
document.querySelector('h1').innerHTML = "A name";
```
and replace "A name" with my name "Ting-Wei".

* **What does the word `document` represent in this code? Explain briefly.**

'document' refers to 'document object' in this code. According to w3schools.com(https://www.w3schools.com/jsref/dom_obj_document.asp), when an HTML document is loaded into a web browser, it becomes a document object. The document object is the root node of the HTML document.

* **What is happening in line 12 (
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

 This will assign the HTML content of the first element with id="items' in the document to the length of the list containing the elements with a specified tag name 'li'.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

The color would be white.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

The style of paragraphs have been defined with borders, background color, padding, font size and line height in between the <style> tags, within the p curly brackets(p{}). In order to change the background color of the paragraph to a different color, we can change the color code of **background-color** attribute in the p curly brackets, such as
	```js
	background-color: #3399ff
	```

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

I created(sort of mimicked) a new function called ```copyFunction_canada()```which first assign the element with id="Canada" to a text "O Canada". I also insert and call out this function on "McGill University" by adding ```oncopy="copyFunction_canada()"``` within the "li" tag. I figured this out by referring and mimicking what is performed to the original copyFunction() in the code and the ```oncopy="copyFunction()"``` code within the "li" tag associated with 'University of Michigan', which is intuitivetly telling me that on copy, call such function. I also noticed at the bottom of the code, there's a place to appear the text within the "div" tags, so I also added one that refers to the id that the result of "0 Canada" from ```copyFunction_canada()``` should appear.
* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```

handleClick() defines what should be called when clicking, and in this piece of code, handleClick() would elicit the alert("hello") function when being clicked. The second part of the code defines a button with <button> tags, and giving the word to appear on the button as "wow". The "onclick=handleClick() id="wow-button" within the button tag will then trigger the handleClick() function when clicking on the button, and thus call out the alert("hello") function.

* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**



### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

Because the following code in the file has set the style for good or error between the <style> tags:
```js
<style type="text/css">
    .error{
        color: red;      //Errors are in red
    }
    .good {
        color: blue;    //Valid inputs are in blue
    }
</style>
```

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

After we googled this line, it tells us this line defines a regular expression to specify what kind of result would be accepted as a correct 'answer'. If the input is the right format as we defined, it will be show "Nice". If the input is not in such format, it will show 'Not valid!'.
Google: /^[a-zA-Z]+$/ means a word with the format of one or more characters consists of a-z or A-Z.

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

The general format of if-else conditional statements in Javascript is something like the following piece of code:
```js
if (condition) {
  //  block of code to be executed if true
} else {
  //  block of code to be executed if false
}
```
The syntax in Javascript are very similar to Python. One of the difference is that in Javascript, the conditional codes to be executed should be wrapped within curly brackets. In Python, we only use colon to indicate the code to be executed. Another difference is that in Python, indentation matters for 'if:' and 'else:' blocks of codes, but in Javascript, we just add curly brackets after if or else.


* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

'10000' refers to the speed of the fading effect in milliseconds.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
    $("form").submit(function(event){
```
(Based on https://www.w3schools.com/jquery/event_ready.asp and https://www.w3schools.com/jquery/jquery_ref_events.asp)
The ready function is to make the "function()" available after the document is loaded and "function()" indicates which function to run after the document is loaded. The second line of code has an "Event method" that triggers or attaches a function to an event handler for selected elements. Then, the submit event will be attached.

* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.
