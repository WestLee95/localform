# Local Storage Form Demo

This project demonstrates how to use local storage in a web application to persist user data temporarily across pages.

## Features

- A simple form to input a user's first and last name.
- Data is stored in the browser's local storage upon form submission.
- A second page retrieves and displays the stored data dynamically.

## Project Structure

- **index.html**: Contains the form for inputting user data.
- **next.html**: Displays the data retrieved from local storage.

## Technologies Used

- **HTML5**: For the structure of the web pages.
- **Tailwind CSS**: For styling the user interface.
- **JavaScript**: For handling form submissions, local storage operations, and navigation.

## Usage Instructions

1. Open `index.html` in your browser.
2. Fill in the "First Name" and "Last Name" fields.
3. Click on the "Next Page" button to submit the form.
4. The `next.html` page will open, displaying the stored data.
5. Use the "Home" button on the `next.html` page to return to the form.

## Code Highlights

- **Data Storage**:  
  The `localStorage.setItem` method is used to save data entered in the form.
- **Data Retrieval**:  
  The `localStorage.getItem` method retrieves the stored data to be displayed on the second page.

### Example Code Snippets

**Storing Data:**
```javascript
localStorage.setItem('first-name', firstNameValue);
localStorage.setItem('last-name', lastNameValue);
```

**Retrieving Data:**
```javascript
document.getElementById('first-name').textContent = localStorage.getItem('first-name');
document.getElementById('last-name').textContent = localStorage.getItem('last-name');
```

## Future Enhancements

- Add input validation for the form fields.
- Implement session storage as an alternative to local storage.
- Introduce additional styling and animations for improved user experience.
