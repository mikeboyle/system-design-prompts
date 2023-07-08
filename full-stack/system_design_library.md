# System Design Intervew: Library System
You've been asked to design a web application for a library.

Consider the information and user stories below, and describe how your software would work.

This is not a coding exercise but you will probably want to sketch or type some things.

There are many ways to succeed at this challenge. You may want to consider the database schema, API endpoints, front end architecture (screens, global state, component hierarchy), or infrastructure.

## Key Requirements
The library software has two main functions. See `Resources` and `User stories` below for more details.

1. Keep track of which books it has, and which are available.
1. Allow library users to check out and return books.

## Resources
The library needs to keep track of **books** and **users** (and maybe other things!)

A **book** has a _title_, _author_, and _ISBN number_ (and maybe other things!).
Every book also has a _category_, which for now is either `"children"` or `"general"`. 
Also important: The library may have multiple copies of the same book.

A **user** has a _name_, _id number_, and _username_ (and maybe other things!).
If a user is younger than 10, they are a child user.
If a user is between 10 and 18, they are a student user.
If a user is over 18 years old, they are an adult user.

## User stories

### Viewing the collection
1. As a user, I want to see all of the library's books.
1. As a user, I want to filter books by category and/or availability.
1. As a user, I want to see books with a specific author, title, or ISBN number.

### Checking out books
1. As a child user, I can check out up to 5 **children's** books for up to 2 weeks per book.
1. As a child user, I cannot check out general books.
1. As a student user, I can check out up to 5 books (children or general) for up to 2 weeks per book.
1. As an adult user, I can check out up to 3 books (children or general) for up to 1 week per book.
1. As a user, I want to see which books I've checked out and when they are due.
1. As a user, I should not be able to see what other users have checked out.

### Returning books
1. When a book is returned, it should become available again.

### Bonus user stories
1. As an admin user, I want to see all the overdue books from all users.
1. As a user, I want to see a history of every book I have checked out (current and past).
1. As a user, I want to reserve a book that is not available.
1. As a user, I want to join a waitlist for an unavailable book and see my place in the waitlist.
1. As a user, I want to see and check out books from multiple library branches in my city.


