# Readings: Object-Oriented Programming, HTML Tables


## Domain Modeling

## Explain why we need domain modeling.
A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.


## HTML Table Basics

## Why should tables not be used for page layouts?
HTML tables should be used for tabular data.
Layout tables reduce accessibility for visually impaired users: screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.
Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug. 
Tables are not automatically responsive: When you use proper layout containers (such as <header>, <section>, <article>, or <div>), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.

## List and describe 3 different semantic HTML elements used in an HTML <table>.
table,th, and td

## Introducing Constructors

## What is a constructor and what are some advantages to using it?
Constructors are a special method of a class for creating and initializing an object instance of that class.

## How does the term this differ when used in an object literal versus when used in a constructor?
A function's this keyword behaves a little differently in JavaScript compared to other languages.  Inside a function, the value of this depends on how the function is called. Think about this as a hidden parameter of a function — just like the parameters declared in the function definition, this is a binding that the language creates for you when the function body is evaluated.
A constructor belongs to a particular class object that is instantiated. The constructor initializes this object and can provide access to its private information. The concept of a constructor can be applied to most object-oriented programming languages. Essentially, a constructor in JavaScript is usually declared at the instance of a class.

## Object Prototypes Using A Constructor

## Explain prototypes and inheritance via an analogy from your previous work experience.
A prototype is just a property that every function in JavaScript has which allows us to share methods across all instances of a function. All our functionality is still the same but now instead of having to manage a separate object for all the methods, we can just use another object that comes built into the function itself.
Inheritance controls what happens when no value is specified for a property on an element.
