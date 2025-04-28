# Calculator App: A Frontend Implementation

This project is a simple calculator web application built using HTML, CSS, and JavaScript. It provides basic arithmetic operations and a user-friendly interface.

## Problem Statement

Create a functional calculator with the following features:

*   Accept numerical inputs from button clicks.
*   Display the current operand and the previous operand/operation.
*   Perform addition, subtraction, multiplication, and division.
*   Handle decimal inputs.
*   Provide "Clear" (AC) and "Delete" (DEL) functionalities.
*   Format the output with commas for large numbers.

## File Structure

*   `index.html`:  The main HTML file containing the structure of the calculator.
*   `styles.css`:  The CSS file responsible for the calculator's styling and layout.
*   `script.js`:  The JavaScript file containing the logic for the calculator's functionality.

## Code Explanation

### `index.html`

*   Defines the basic HTML structure of the calculator, including the display area and buttons.
*   Uses a `calculator-grid` class for layout using CSS Grid.
*   Each button is assigned a `data-*` attribute for easy selection and functionality binding in JavaScript.

### `styles.css`

*   Provides the visual styling for the calculator.
*   Uses CSS Grid to create the calculator layout.
*   Styles the buttons, output display, and other elements for a clean and user-friendly interface.

### `script.js`

*   Contains the core logic for the calculator.
*   **`Calculator` Class:**
    *   `constructor(previousOperandTextElement, currentOperandTextElement)`: Initializes the calculator with references to the display elements.
    *   `clear()`: Resets the calculator to its initial state.
    *   `delete()`: Removes the last digit from the current operand.
    *   `appendNumber(number)`: Appends a number to the current operand, handling decimal points.
    *   `chooseOperation(operation)`: Selects an operation, moving the current operand to the previous operand and preparing for the next input.
    *   `compute()`: Performs the calculation based on the selected operation.
    *   `getDisplayNumber(number)`: Formats the number for display, adding commas for thousands separators.
    *   `updateDisplay()`: Updates the display elements with the current and previous operands and operation.

*   **Event Listeners:**
    *   Attaches event listeners to each button to handle clicks.
    *   Calls the appropriate `Calculator` class methods based on the button clicked.

## How to Run

1.  Save all the files (`index.html`, `styles.css`, `script.js`) in the same directory.
2.  Open `index.html` in any web browser.

## Sample Usage

1.  Click on the number buttons to enter the first operand.
2.  Click on an operation button (+, -, \*, ÷) to select the desired operation.
3.  Click on the number buttons to enter the second operand.
4.  Click the "=" button to calculate the result.
5.  Click the "AC" button to clear the calculator.
6.  Click the "DEL" button to delete the last digit.

## Enhancements

*   Implement keyboard support.
*   Add more advanced functions (e.g., square root, percentage).
*   Implement error handling for division by zero.
*   Improve the UI/UX with better styling and animations.
*   Add memory functions (M+, M-, MR, MC).
