# Local Library Express project

## This project is done to setup an Express project and learn about its environment and components.

## The project would include :

- Use the Express Application Generator tool to create a skeleton website and application.
- Start and stop the Node web server.
- Use a database to store your application's data.
- Create routes for requesting different information, and templates ("views") to render the data as HTML to be displayed in the browser.
- Work with forms.
- Deploy your application to production.

## Descriptioin

LocalLibrary is the name of the website that we'll create and evolve over the course of this series of tutorials. As you'd expect, the purpose of the website is to provide an online catalog for a small local library, where users can browse available books and manage their accounts.

This example has been carefully chosen because it can scale to show as much or little detail as we need, and can be used to show off almost any Express feature. More importantly, it allows us to provide a guided path through the functionality you'll need in any website:

- In the first few tutorial articles we will define a simple browse-only library that library members can use to find out what books are available. This allows us to explore the operations that are common to almost every website: reading and displaying content from a database.
- As we progress, the library example naturally extends to demonstrate more advanced website features. For example we can extend the library to allow new books to be created, and use this to demonstrate how to use forms, and support user authentication.

Even though this is a very extensible example, it's called LocalLibrary for a reason — we're hoping to show the minimum information that will help you get up and running with Express quickly. As a result we'll store information about books, copies of books, authors and other key information. We won't however be storing information about other items a library might lend, or provide the infrastructure needed to support multiple library sites or other "big library" features.