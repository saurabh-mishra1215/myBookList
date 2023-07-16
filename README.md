# myBookList
This is my book list app
The code provided represents a simple book tracking application that allows users to add and remove books from a list.
Here's a breakdown of how the code works:

1. The `Book` class represents a book object with properties like title, author, and ISBN.

2. The `UI` class handles UI-related tasks such as displaying books, adding books to the UI, deleting books from the UI, showing alerts, and clearing input fields.

3. The `Store` class handles storage-related tasks using the browser's `localStorage`. It provides methods to get books from storage, add a book to storage, and remove a book from storage.

4. The `DOMContentLoaded` event listener calls the `displayBooks` method from the `UI` class to populate the UI with books stored in the `localStorage` when the page loads.

5. The `submit` event listener on the book form captures the form submission, retrieves the input values for title, author, and ISBN, validates the input, creates a new `Book` object, adds the book to the UI using the `addBookToList` method from the `UI` class, stores the book using the `addBook` method from the `Store` class, shows a success message using the `showAlert` method from the `UI` class, and clears the input fields.

6. The `click` event listener on the book list captures the click event on the delete button, removes the book from the UI using the `deleteBook` method from the `UI` class, removes the book from storage using the `removeBook` method from the `Store` class, and shows a success message using the `showAlert` method from the `UI` class.

Overall, this code provides a basic implementation for managing a list of books in the browser's `localStorage`.
