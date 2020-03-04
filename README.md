# Bible-database-for-python
A collection of `The Holy Bible` in various languages used for a python program

The `Bibles` in this collection are in the database format and can be opened using `sqlite` module.

## Schema
Each Bible has 2 tables. The schema is given below:

Table 1: `CREATE TABLE "bible" ("Book"	INTEGER, "Chapter"	INTEGER, "Versecount"	INTEGER, "verse"	TEXT)`
Table 2: `CREATE TABLE "bookIndex" ( "num" INTEGER, "name" TEXT )`

Any future commits has to follow this schema strictly.

## Explanation of Schema
### Table 1:
`Book` starts with 0 and ends with 65 - all integers
`Chapter` starts with 1 and ends with the number of chapter in the respective books
`Versecount` starts with 1 and ends with the last verse number of each chapter
`verse` contains the text of the verse
### Table 2:
`num` indicates the book number
`name` gives the book name in the given language

This table is used to get the name of books in the language of the Bible


