# CinemaSeating
A command-line program for managing seating allocation for a movie theatre, developed with emphasis on a test-driven development approach. The movie theatre has fifteen seats, arranged in three rows of five seats. Each row is assigned a letter from A to C, and each seat has a number from 1 to 5.

<br/>

## User Stories
User stories describe the expected behaviour of a system from the perspective of the end-user, which provides a better understanding of how the final product should behave and allows developers to prioritise core functionalities.
The expected end-user will be a Cinema Manager who is tasked with allocating seats for various viewings using the program.

<br/>

#### User Story 1
"As a Cinema Manager I want to allocate seats to customers so that I can control reserved seating for the theatre"

- <b>GIVEN</b> a customer wants to request some tickets

- <b>WHEN</b> they request a number of seats between 1 and 3 for a movie

- <b>THEN</b> the customer should be allocated the required number of seats
from the available seats on the seating plan

- <b>AND</b> the seats should be recorded as allocated

<br/>

#### User Story 2
"As a Cinema Manager I want to check seat availability between each booking so that I can prevent overbooking seats that have already been allocated"

- <b>GIVEN</b> a seat is allocated

- <b>WHEN</b> a customer has successfully requested a number of seats

- <b>THEN</b> the program should record which seats and rows are still available

- <b>AND</b> display them in a readable format after each booking

<br/>

#### User Story 3
"As a Cinema Manager I want to be able to see how many seats have been sold so that I can track revenue for the movie"

- <b>GIVEN</b> a customer requests a number of seats that cannot be allocated

- <b>WHEN</b> the program halts and returns the final seat allocation report

- <b>THEN</b> the program should calculate the sum of allocated seats

- <b>AND</b> display the sum so that I can use it to calculate revenue


<br/>

## Requirements

#### Functional

- Allocate seats based on a random integer (number of seats) between 1 and 3
- Allocate seats starting from A1 and fill from left to right, front to back
- Every seat will be available when the program starts
- Continue to allocate a random number of seats until there are not enough seats left to complete the request
  - The program will stop when this condition is met


#### Non-functional

- Demonstrate a clear, test-driven approach with descriptive test cases
- Implement separation of concerns and single responsibility principle
- Adhre to SOLID principles
- Provide a user-friendly command-line interface
- Record the seat status when the program halts, indicating which seats are allocated and which are available
  - (e.g. "A1: Allocated", "A2: Available", etc.)
- Display informative error messages
- Test cases cover various scenarios, including seat allocation success, failure, errors and exceptions


<br/>

## Testing
