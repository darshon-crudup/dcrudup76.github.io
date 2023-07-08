## Component-Based Architecture

Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides the problem into sub-problems, each associated with component partitions.

The primary objective of component-based architecture is to ensure component reusability. A component encapsulates functionality and behaviors of a software element into a reusable and self-deployable binary unit. There are many standard component frameworks such as COM/DCOM, JavaBean, EJB, CORBA, .NET, web services, and grid services. These technologies are widely used in local desktop GUI application design such as graphic JavaBean components, MS ActiveX components, and COM components which can be reused by simply drag and drop operation.

Component-oriented software design has many advantages over the traditional object-oriented approaches such as −

Reduced time in market and the development cost by reusing existing components.
Increased reliability with the reuse of the existing components.

React has a different approach to data flow & manipulation than other frameworks, and that’s why it can be difficult at the beginning to understand some concepts like props, state, and so on.

I believe it’s better to keep explaining them in separate posts and in this article, we’re going to focus on React’s Props feature and how to use it.
To understand how props work, first, you need to have a general understanding of the concept of the components. If you don’t know much about components in React, I recommend reading my previous article about React components.

# What is Props?
React is a component-based library that divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.

“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)
Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.

# Recap:
Props stand for properties and is a special keyword in React
Props are being passed to components like function arguments
Props can only be passed to components in one way (parent to child)
Props data is immutable (read-only)



# What is a “component”?
A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.
# What are the characteristics of a component?
Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.
Replaceable − Components may be freely substituted with other similar components.
Not context specific − Components are designed to operate in different environments and contexts.
Extensible − A component can be extended from existing components to provide new behavior.
Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
Independent − Components are designed to have minimal dependencies on other components.
# What are the advantages of using component-based architecture?
Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.
Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.
Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.
Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

## What is Props and How to Use it in React

# What is “props” short for?
React is a component-based library that divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.
“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

# How are props used in React?
Props define an attribute and its value(data),then pass it to child component(s) by using Props, and render the Props Data.
# What is the flow of props?
Props are being passed in a uni-directional flow. (one way from parent to child)
