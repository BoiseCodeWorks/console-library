# Console-Library

Diving into the world of C# can be overwhelming... So let's build a checkout system for a couple of our favorite books.

This will be a console app that will provide users a choice of books to checkout. Because we have a limited supply of books you will limit the books that a user can check out at a time to 1. With this rule in mind users need a way to check a book back into the library. 

```terminal
Select a Book to Checkout:

1. HeadFirst with C#
2. Mastering the Console App
3. C# Game Programming: For Serious Game Creation
4. Pro C# 5.0 and the .NET 4.5 Framework
5. Return Book

Select the Book you would like to checkout by number: 
```

To Get started create a `new Console Application` from Visual Studio or use the [yo generator](https://www.npmjs.com/package/generator-aspnet)

You will need two classes 

`Book.cs`

```c#
public class Book
{
    public string Title;
    public string Author;
}
```

`Library.cs`

```c#
public class Library
{
    public List<Book> Books = new List<Book>();
}
```

Think about how you will need to instantiate these objects. 

How do you create a `new Library` that can have a list of books?

You will also need a couple of Methods that you can call from Program.cs

### Checkout()
The Checkout Method should be responsible for removing a book from the `List` of `AvailableBooks`.

### SelectBook()
SelectBook will need to check the users input and validate the input is a valid

### ReturnBook()
Responsible for adding a previously checked out book to be returned to the `List` of `AvailableBooks`

### Bonus Challenge
When a book is returned display to the console the amount of time the book was absent for.
