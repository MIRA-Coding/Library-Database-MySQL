# Library Database Management 📚🏫

## Description
This project is a database management system designed for library operations. 
It includes structured data files for storing and managing information related 
to books, authors, customers, and their contact information. 
The database is implemented using MySQL and supports essential operations for a library system.

## Files in the Project

### `author.ibd`
- Stores data about authors of books.
- Fields include:
  - Author_ID
  - fname
  - lname
  - midname
  - DOB "Date Of Birth"

### `book.ibd`
- Contains information about the books in the library.
- Fields include:
  - book_title
  - publish_year
  - book_ID
  - price
  - language
  - author_ID
  - publisher_ID

### `customer.ibd`
- Holds data related to library customers.
- Fields include:
  - customer_ID
  - fname
  - lname
  - Email
  - wishlist_ID

### `cphone_no.ibd`
- Stores contact numbers for customers.
- Fields include:
  - customer_ID
  - phone_No
 
### `order.ibd`
- Stores orders of customers.
- Fields include:
  - order_ID
  - order_status
  - order_date
  - quantity
  - customer_ID
 
 ### `orderbooks.ibd`
- serving as a junction table for a many-to-many relationship between the `book` and `order` tables. 
- This design is necessary because:
  - enables efficient **normalization** of the database by avoiding redundancy simplifying the querying
- Fields include:
  - book_ID
  - order_ID
 
### `publisher.ibd`
- Stores publisher details.
- Fields include:
  - publisher_ID
  - name
  - contactDetails

## Usage
1. Ensure that MySQL is installed on your system.
2. Import these `.ibd` files into the appropriate MySQL database instance.

## Future Enhancements
- add more table to complete the Commercial Library System
- add the .sql file so you can run it by you own.

if any request let me know 🤝
