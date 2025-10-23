CREATE DATABASE bookstore;
USE bookstore;
CREATE TABLE Authors (
    author_id INT PRIMARY KEY AUTO_increment,
    name VARCHAR(100) NOT NULL,
    country VARCHAR(50)
);
CREATE TABLE Books(
    book_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(150) NOT NULL,
    published_year INT,
    author_id INT,
    FOREIGN KEY (author_id) REFERENCES Authors(authot_id)
);
DESCRIBE Authors;
DESCRIBE Books;
DROP TABLE books;
---re-createb books table
CREATE TABLE Books(
    book_id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(150) NOT NULL,
    published_year INT,
    author_id INT,
    FOREIGN KEY (author_id) REFERENCES Authors(author_id)
);
DROP DATABASE bookstors;
---re-create the database
CREATE DATABASE bookstore;
USE bookstore;
CREATE TABLE Authors (
    authors_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    country VARCHAR(50)
);
CREATE TABLE Books(
    book_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(150) NOT NULL,
    published_year INT,
    author_id INT,
    FOREIGN KEY (author_id) REFERENCES Authors(authot_id)
);
---Insert Data "day 13"
INSERT INTO Authors (name,country)
VALUES
('J.K.ROWLING', 'UK'),
('Geaorge R.R.Martin', 'USA'),
('Haruki Murakami','Japan');
INSERT INTO books (title,published_year,author_id)
VALUES
('Harry Potter and the philosopher''s stone',1997,1),
('A Game of Thrones',1996,2),
('Kafla on the shore',2002,3),
('Norwegain Wood',1987,3);
---Query Data
SELECT * FROM Authors;
SELECT * FROM Books;
SELECT title FROM Books WHERE published_year>1990;
SELECT title,published_year FROM Books WHERE author_id in (select author_id from Authors where name='Haruki Murakami');
---Update Data
UPDATE books SET published_year=1989 WHERE title='Norwegian Wood ';
UPDATE Authors SET country='United kingdom' WHERE name= 'j.k.Rowling';
---Delete Data
DELETE FROM books WHERE title='kafka on the shore';
---D'ABORT ON SUPPRIME GEORGE R.R.MARTIN DE LA TABLE DE BOOKS 
DELETE FROM books WHERE author_id=(SELECT author_id FROM Authors WHERE name='George R.R.Martin');
DELETE FROM Authors WHERE name='George R.R.Martin';










    








