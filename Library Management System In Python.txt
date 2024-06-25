"""
Task:

Make A library Management System:

Steps:

1. Make 2 instance variables "books" and "no_of_books"

2. The "books" is an empty list.

3. The no_of_books is an integer equal to zero.

4. Make another instance method.

5. This instance method takes a new book as an argument and each time I call this function
   and pass a new argument it appends that argument to the books list.

6. Now Create a library for Library class( i.e : object reference ).

7. Now using that library print the number of books passed as an argument to the previous instance
   method by incrementing the value of the variable no_of_books.

8. Also print it using the length of the list of books.

9. Now print the all the books passed as an argument.

"""

class Library:

    def variables(self):
        self.no_of_books = 0
        self.books = []

    def show_books(self, books_Available):
        self.books.append(books_Available)
        self.no_of_books = len(self.books)


library = Library()
library.variables()
library.show_books("Hacking")
library.show_books("Django")
library.show_books("python")
library.show_books("rucky")
library.show_books("fing")
print(f"The Books In The Libreary Are: {library.books}")
print(f"The Number of Books In Library Are: {len(library.books)} ")
print(f"The Number of Books In Library Are: {library.no_of_books} ")

