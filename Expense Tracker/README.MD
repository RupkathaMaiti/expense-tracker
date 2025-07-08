Expense Tracker
This is a web-based Expense Tracker application designed to help users manage their finances by allowing them to input their expenses and income, categorize transactions, and view a summary of their financial activities.

Table of Contents
Features

Technologies Used

Setup and Installation

How to Use

Project Structure

Responsiveness

Persistence

Bonus Features

Features
User-Friendly Interface: A clean and intuitive web interface for easy navigation.

Transaction Management:

Add new income and expense transactions.

Input fields for Date, Description, Category, Amount, and Type (Income/Expense).

Categorize transactions (e.g., Food, Transportation, Entertainment, Salary, etc.).

Display a list of all transactions with their details.

Edit existing transactions via a modal.

Delete individual transactions.

Financial Summary:

Calculates and displays total income.

Calculates and displays total expenses.

Calculates and displays net income (Total Income - Total Expenses).

Input Validation: Basic validation ensures that all required fields are filled and amounts are positive numbers.

Data Persistence: Transactions are saved locally in the browser's Local Storage, so your data remains even after closing and reopening the application.

Filtering: Filter transactions by category.

Data Visualization: A pie chart visualizes the distribution of expenses by category.

Data Export/Import: Export your transaction data to a JSON file or import data from a JSON file.

Rupee Currency: All monetary values are displayed in Indian Rupees (₹).

Technologies Used
HTML5: For the structure and content of the web application.

CSS3 (Tailwind CSS): For styling the application and ensuring a responsive design.

Tailwind CSS is loaded via CDN.

JavaScript (ES6+): For all interactive functionalities, data management, and calculations.

Chart.js: Used for creating the expense distribution pie chart (loaded via CDN).

Setup and Installation
This project is a single-page web application and does not require any complex setup or build process.

Download the files: Save the provided HTML code (which includes embedded CSS and JavaScript) as index.html.

Open in Browser: Simply open the index.html file in any modern web browser (e.g., Chrome, Firefox, Edge, Safari).

The application will run directly in your browser.

How to Use
Add a Transaction:

Fill in the Date, Description, Category, Amount, and select the Type (Expense or Income).

Click the "Add Transaction" button.

View Transactions:

All added transactions will appear in the "Transactions" table below the input form.

Transactions are sorted by date, with the most recent at the top.

Summary Overview:

The "Total Income," "Total Expenses," and "Net Income" cards at the top will update automatically with each transaction.

Edit a Transaction:

Click the "Edit" button next to the transaction you wish to modify in the table.

A modal window will appear with the transaction's details. Update the fields as needed.

Click "Save Changes" to apply the updates or "Cancel" to discard them.

Delete a Transaction:

Click the "Delete" button next to the transaction you wish to remove from the table.

Filter Transactions:

Use the "Filter by Category" dropdown above the transactions table to view transactions belonging to a specific category or "All Categories".

Expense Distribution Chart:

A pie chart at the bottom of the page visualizes how your expenses are distributed across different categories.

Export Data:

Click the "Export Data" button to download your current transaction data as a expense_tracker_data.json file.

Import Data:

Click the "Import Data" button. A file selection dialog will appear.

Select a previously exported expense_tracker_data.json file to load its contents into the tracker, replacing any existing data.

Project Structure
The entire application is contained within a single index.html file, which includes:

HTML Structure: Defines the layout of the Expense Tracker, including input forms, summary cards, transaction table, and chart canvas.

CSS Styling: Embedded within the <style> tags, it uses Tailwind CSS classes and custom CSS to provide a responsive and visually appealing design.

JavaScript Logic: Embedded within the <script> tags, it handles all the application's functionality:

Managing transaction data (add, edit, delete).

Updating summary calculations.

Rendering transactions in the table.

Handling local storage for data persistence.

Filtering transactions.

Updating the expense distribution chart.

Implementing export and import functionalities.

Managing the edit modal and input validation.

Responsiveness
The application is designed to be fully responsive and provides a good user experience across various screen sizes, including desktops, tablets, and mobile phones. This is achieved through:

Viewport Meta Tag: Ensures proper scaling on different devices.

Flexbox and Grid Layouts: Used for flexible and adaptable component arrangements.

Tailwind CSS Responsive Utilities: Utilizes Tailwind's breakpoint prefixes (sm:, md:, lg:) to adjust styles based on screen size.

Overflow Handling: The transaction table includes horizontal scrolling on smaller screens to prevent layout breakage.

Persistence
The application uses the browser's localStorage to store transaction data. This means that:

Your transactions will be saved even if you close the browser tab or window.

The data will be available the next time you open the application in the same browser.

Bonus Features
Category Filtering: Easily filter transactions by category using a dropdown.

Data Visualization: A dynamic pie chart provides a visual representation of your spending habits across different expense categories.

Edit Functionality: Users can modify existing transactions, correcting errors or updating details.

Export/Import: Provides flexibility for users to back up their data or transfer it between devices.