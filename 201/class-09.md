# Readings: Forms and JS Events

## HTML Forms

## Why are forms so important in web development?
Web forms are one of the main points of interaction between a user and a website or application. Forms allow users to enter data, which is generally sent to a web server for processing and storage or used on the client-side to immediately update the interface in some way.  A web form's HTML is made up of one or more form controls, plus some additional elements to help structure the overall form — they are often referred to as HTML forms.

When designing a form, what are some key things to keep in mind when it comes to user experience?
From a user experience (UX) point of view, it's important to remember that the bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.

## List 5 form elements and explain their importance.
The li elements are there to conveniently structure our code and make styling easier.
The <input> element, the most important attribute is the type attribute. This attribute is extremely important because it defines the way the <input> element appears and behaves. 
The button element adds a button to allow the user to send, or "submit", their data once they have filled out the form. 
The <output> HTML element is a container element into which a site or app can inject the results of a calculation or the outcome of a user action.
The <form> HTML element represents a document section containing interactive controls for submitting information.

## Learn JS

## Introduction To Events.

## How would you describe events to a non-technical friend?
Events are actions or occurrences that happen in the system you are programming, which the system tells you about so your code can react to them.
For example, if the user clicks a button on a webpage, you might want to react to that action by displaying an information box. 

## When using the addEventListener() method, what 2 arguments will you need to provide?
Objects that can fire events have an addEventListener() method, that takes at least two arguments: the name of the event and a function to handle the event. 

## Describe the event object. Why is the target within the event object useful?
Inside an event handler function, you'll see a parameter specified with a name such as event, evt, or e. This is called the event object, and it is automatically passed to event handlers to provide extra features and information.  The target property of the event object is always a reference to the element the event occurred upon.

## What is the difference between event bubbling and event capturing?
Event bubbling describes how the browser handles events targeted at nested elements.
An alternative form of event propagation is event capture. This is like event bubbling but the order is reversed: so instead of the event firing first on the innermost element targeted, and then on successively less nested elements, the event fires first on the least nested element, and then on successively more nested elements, until the target is reached.
