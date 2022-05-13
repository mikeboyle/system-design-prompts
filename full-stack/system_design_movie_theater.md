# System Design Intervew: Movie Theater Ticketing
You've been asked to design a web application for a movie theater.

Consider the requirements and user stories below, and describe how your software would work.

This is not a coding exercise but you will probably want to sketch or type some things.

There are many ways to succeed at this challenge. You may want to consider the database schema, API endpoints, front end architecture (screens, global state, component hierarchy), or infrastructure.

## Key Requirements
The movie theater software has two main functions. See `Resources` and `User stories` below for more details.

1. Set and display a schedule of movie screenings
1. Sell movie tickets to customers

You may assume that details like user authentication and payment processing will be handled by another part of the system that we're not responsible for building.

## Resources
The client knows they need to keep track of the following things ... and maybe other things!

1. A **movie** has a _title_, _rating_, and _running time_ (number of minutes).
1. This is a multiplex theater so there are many **auditoriums**. An auditorium has a _number_ that customers and staff use to identify it.
1. Each auditorium has many **seats** that are identified by _row number_ and _seat number_.
1. The theaters sells **tickets** that are for a specific seat for a specific screening (a showing of a movie at a certain auditorium at a certain time). Tickets have different _prices_ for adults and children.

## User stories

### As a customer, ...
1. I can see all of the movies and showtimes for today.
1. I can see whether a particular screening has seats available.
1. I can see which seats are available for a specific screening.
1. I can purchase a ticket for a seat at a specific screening.
1. I can purchase up to 5 tickets at one time.

### As a theater admin, ...
1. I can set which movies are showing at the theater.
1. I can schedule screenings for today and the next 30 days.
1. I can manage (change or delete) movies and screenings.
1. I can see how much money we have made in tickets sales.

### Bonus user stories
1. As a user, I can view my purchase history (past tickets and upcoming shows).
1. As a user, I can select seats and have 5 minutes to complete my purchase. During that time no other user can select or purchase a ticket for that seat.
1. As a theater admin, I have a way to "check in" a customer who presents a ticket. (For example, I can check the customer's user id against the purchase.)
1. The movie theater is so successful that they want to expand to multiple locations. How does the software need to change to support this?


