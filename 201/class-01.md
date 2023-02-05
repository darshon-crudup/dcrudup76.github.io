# HTML

## What is HTML?

HTML (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit. It can be as complicated or as simple as the web developer wants it to be. HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way. The enclosing tags can make content into a hyperlink to connect to another page, italicize words, and so on. For example, consider the following line of text:

My cat is very grumpy
If we wanted the text to stand by itself, we could specify that it is a paragraph by enclosing it in a paragraph (<p>) element:

<p>My cat is very grumpy</p>

## How the web works

Overview: Getting started with the web
How the web works provides a simplified view of what happens when you view a webpage in a web browser on your computer or phone.

This theory is not essential to writing web code in the short term, but before long you'll really start to benefit from understanding what's happening in the background.

## Clients and servers
Computers connected to the internet are called clients and servers.

Two circles representing client and server. An arrow labelled request is going from client to server, and an arrow labelled responses is going from server to client.

Clients are the typical web user's internet-connected devices (for example, your computer connected to your Wi-Fi, or your phone connected to your mobile network) and web-accessing software available on those devices (usually a web browser like Firefox or Chrome).

Servers are computers that store webpages, sites, or apps. When a client device wants to access a webpage, a copy of the webpage is downloaded from the server onto the client machine to be displayed in the user's web browser.

## What will your website look like?

Overview: Getting started with the web

What will your website look like? discusses the planning and design work you have to do for your website before writing code, including "What information does my website offer?", "What fonts and colors do I want?", and "What does my site do?"

## First things first: planning

Before doing anything, you need some ideas. What should your website actually do? A website can do basically anything, but, for your first try, you should keep things simple. We'll start by creating a simple webpage with a heading, an image, and a few paragraphs.

To begin, you'll need to answer these questions:

1. What is your website about? Do you like dogs, New York, or Pac-Man?

2. What information are you presenting on the subject? Write a title and a few paragraphs and think of an image you'd like to show on your page.

3. What does your website look like, in simple high-level terms? What's the background color? What kind of font is appropriate: formal, cartoony, bold and loud, subtle?

## Sketching out your design

Next, grab pen and paper and sketch out roughly how you want your site to look. For your first simple webpage, there's not much to sketch out, but you should get in the habit of doing this now. It really helps — you don't have to be Van Gogh!

## Images

To choose an image, go to Google Images and search for something suitable.

When you find the image you want, click on the image to get an enlarged view of it.

Right-click the image (Ctrl + click on a Mac), choose Save Image As…, and choose a safe place to save your image. Alternatively, copy the image's web address from your browser's address bar for later use.

## Search results for a search term on Google Images

Note that most images on the web, including in Google Images, are copyrighted. To reduce your likelihood of violating copyright, you can use Google's license filter. Click on the Tools button, then on the resulting Usage rights option that appears below. You should choose the option Creative Commons licenses.

## What is JavaScript?

JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved. It is the third layer of the layer cake of standard web technologies, two of which (HTML and CSS) we have covered in much more detail in other parts of the Learning Area.

## The three layers of standard web technologies; HTML, CSS and JavaScript

HTML is the markup language that we use to structure and give meaning to our web content, for example defining paragraphs, headings, and data tables, or embedding images and videos in the page.

CSS is a language of style rules that we use to apply styling to our HTML content, for example setting background colors and fonts, and laying out our content in multiple columns.

JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

## Strings — the basics

Strings are dealt with similarly to numbers at first glance, but when you dig deeper you'll start to see some notable differences. Let's start by entering some basic lines into the browser developer console to familiarize ourselves.

## Creating a string

To start with, enter the following lines:

const string = "The revolution will not be televised.";
console.log(string);

Copy to Clipboard

Just like we did with numbers, we are declaring a variable, initializing it with a string value, and then returning the value. The only difference here is that when writing a string, you need to surround the value with quotes.

If you don't do this, or miss one of the quotes, you'll get an error. Try entering the following lines:

const badString1 = This is a test;
const badString2 = 'This is a test;
const badString3 = This is a test';

These lines don't work because any text without quotes around it is assumed to be a variable name, property name, a reserved word, or similar. If the browser can't find it, then an error is raised (e.g. "missing; before statement"). If the browser can see where a string starts, but can't find the end of the string, as indicated by the 2nd quote, it complains with an error (with "unterminated string literal"). If your program is raising such errors, then go back and check all your strings to make sure you have no missing quote marks.

The following will work if you previously defined the variable string — try it now:

const badString = string;
console.log(badString);

Copy to Clipboard

badString is now set to have the same value as string.

## Numbers vs. strings

So what happens when we try to combine a string and a number? Let's try it in our console:

const name = "Front ";
const number = 242;
console.log(`${name}${number}`); // "Front 242"

Copy to Clipboard

You might expect this to return an error, but it works just fine. Trying to represent a string as a number doesn't really make sense, but representing a number as a string does, so the browser converts the number to a string and concatenates the two strings.

If you have a numeric variable that you want to convert to a string but not change otherwise, or a string variable that you want to convert to a number but not change otherwise, you can use the following two constructs:

The Number() function converts anything passed to it into a number, if it can. Try the following:

const myString = "123";
const myNum = Number(myString);
console.log(typeof myNum);

Copy to Clipboard

Conversely, every number has a method called toString() that converts it to the equivalent string. Try this:

const myNum2 = 123;
const myString2 = myNum2.toString();
console.log(typeof myString2);

Copy to Clipboard

These constructs can be really useful in some situations. For example, if a user enters a number into a form's text field, it's a string. However, if you want to add this number to something, you'll need it to be a number, so you could pass it through Number() to handle this.

What is a variable?
A variable is a container for a value, like a number we might use in a sum, or a string that we might use as part of a sentence.

Variable example
Let's look at a simple example:

<button id="button_A">Press me</button>
<h3 id="heading_A"></h3>

Copy to Clipboard

const buttonA = document.querySelector('#button_A');
const headingA = document.querySelector('#heading_A');

buttonA.onclick = () => {
  const name = prompt('What is your name?');
  alert(`Hello ${name}, nice to see you!`);
  headingA.textContent = `Welcome ${name}`;
}
Copy to Clipboard

In this example pressing the button runs some code. The first line pops a box up on the screen that asks the reader to enter their name, and then stores the value in a variable. The second line displays a welcome message that includes their name, taken from the variable value and the third line displays that name on the page.

Without a variable
To understand why this is so useful, let's think about how we'd write this example without using a variable. It would end up looking something like this:

<button id="button_B">Press me</button>
<h3 id="heading_B"></h3>
const buttonB = document.querySelector('#button_B');
const headingB = document.querySelector('#heading_B');

buttonB.onclick = () => {
    alert(`Hello ${prompt('What is your name?')}, nice to see you!`);
    headingB.textContent = `Welcome ${prompt('What is your name?')}`;
}

You may not fully understand the syntax we are using (yet!), but you should be able to get the idea. If we didn't have variables available, we'd have to ask the reader for their name every time we needed to use it!

Variables just make sense, and as you learn more about JavaScript they will start to become second nature.

One special thing about variables is that they can contain just about anything — not just strings and numbers. Variables can also contain complex data and even entire functions to do amazing things. You'll learn more about this as you go along.

Note: We say variables contain values. This is an important distinction to make. Variables aren't the values themselves; they are containers for values. You can think of them being like little cardboard boxes that you can store things in.

A screenshot of three 3-dimensional cardboard boxes demonstrating examples of javascript variables. Each box contains hypothetical values that represent various javascript data types. The sample values are "Bob", true and 35 respectively.

## Declaring a variable

To use a variable, you've first got to create it — more accurately, we call this declaring the variable. To do this, we type the keyword let followed by the name you want to call your variable:

let myName;
let myAge;

Copy to 

Here we're creating two variables called myName and myAge. Try typing these lines into your web browser's console. After that, try creating a variable (or two) with your own name choices.

Note: In JavaScript, all code instructions should end with a semicolon (;) — your code may work correctly for single lines, but probably won't when you are writing multiple lines of code together. Try to get into the habit of including it.

You can test whether these values now exist in the execution environment by typing just the variable's name, e.g.

myName;
myAge;

Copy to Clipboard

They currently have no value; they are empty containers. When you enter the variable names, you should get a value of undefined returned. If they don't exist, you'll get an error message — try typing in

scoobyDoo;

Copy to Clipboard

Note: Don't confuse a variable that exists but has no defined value with a variable that doesn't exist at all — they are very different things. In the box analogy you saw above, not existing would mean there's no box (variable) for a value to go in. No value defined would mean that there is a box, but it has no value inside it.

Initializing a variable

Once you've declared a variable, you can initialize it with a value. You do this by typing the variable name, followed by an equals sign (=), followed by the value you want to give it. For example:

myName = 'Chris';
myAge = 37;

Copy to Clipboard

Try going back to the console now and typing in these lines. You should see the value you've assigned to the variable returned in the console to confirm it, in each case. Again, you can return your variable values by typing their name into the console — try these again:

myName;
myAge;

Copy to Clipboard

You can declare and initialize a variable at the same time, like this:

let myDog = 'Rover';

Copy to Clipboard

This is probably what you'll do most of the time, as it is quicker than doing the two actions on two separate lines.

## Things I want to know more about
