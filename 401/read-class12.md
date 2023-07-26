## Read: Class 12

# Spring guide: Accessing Data with JPA

1. How are query methods defined when using Spring Data JPA? Query methods are defined by declaring their method signature.
2. Which dependencies will you need in order to complete the Spring guide?  A Spring guide typically requires some common dependencies. These dependencies can vary depending on the specific Spring project and the version you are using such as Spring Boot.
3. What annotations are used to specify an auto generated identification number for an Entity?
In Spring and JPA (Java Persistence API), you can use the @GeneratedValue annotation along with the @Id annotation to specify an auto-generated identification number for an entity.

# Baeldung: Comparing repositories (we’ll be using JpaRepository)

1. Which of the Spring Data Repositories covered in the readings has the most methods available to it?  The JpaRepository is the Spring Data Repository that has the most methods available to it.
2. Name a downstide of a Spring Data Repository.  One downside of using a Spring Data Repository is that it can lead to over-abstraction and complexity in certain scenarios.
3. How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?  To define an operation to find a student based on their name in a repository named StudentRepository that extends JpaRepository, you can use Spring Data's query method feature. Spring Data JPA allows you to create queries directly from method names by following a specific naming convention.

## Things I want to know more about
- Understanding query methods
- Defining operations
