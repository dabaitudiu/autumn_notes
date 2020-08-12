## Design a Library Management System

A Library Management System is a software built to handle the primary housekeeping functions of a library. Libraries rely on library management systems to manage asset collections as well as relationships with their members. Library management systems help libraries keep track of the books and their checkouts, as well as members’ subscriptions and profiles.

Library management systems also involve maintaining the database for entering new books and recording books that have been borrowed with their respective due dates.

### 1. 明确要求

<p align="center">
  <img src="https://github.com/dabaitudiu/autumn_notes/blob/master/OOD/library.png" alt="drawing" width="700"/>
</p>


#### Possible Questions to Ask:

###### Book:

1. What kind of information a book can have?  What is the critical id for a book?

2. Can there be multiple copies of a book? 

###### Person:

1. How can a person search a book? (i.e. use what kind of features)

2. I assume that a person can borrow/return/reserve a book, right?

3. How many books can a person borrow at a time? How long can he borrow?

4. Is there a fining system? How can a person pay fine?

###### System:

1. Is there an online system that can have interactions with a person?
2. Can the system send notice to users?
3. Can people finish borrow/return/reserve/pay fine process through this system?

###### Librarian:
1. I assume a librarian can borrow out, accept return, make reservation, accept fines, right?
2. I assume that a librarian can check/update books info, right?
3. Can a librarian send notification manually?
4. I assume a librarian can check all transactions at any time, right?
