# Palindrome Checker

Welcome to the **Palindrome Checker** repository! This project is a simple web application written in HTML, CSS, and JavaScript. The application allows users to check if a given string is a palindrome.

## Features

- **String Input**: Enter a string to check.
- **Palindrome Validation**: Determine if the input string is a palindrome.
- **Interactive Interface**: Simple and intuitive user interface for easy checking.
- **Responsive Design**: Optimized for both desktop and mobile devices.

## Technologies

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla JS)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/palindrome-checker.git
   cd palindrome-checker
   ```

2. **Open the index.html file**:
   - You can open the `index.html` file directly in your web browser to use the Palindrome Checker.

## Usage

1. Open the Palindrome Checker in your web browser.
2. Enter a string in the input field.
3. Click the button to check if the string is a palindrome.
4. The result will be displayed indicating whether the string is a palindrome or not.

## Project Structure

- `index.html`: The main HTML file for the Palindrome Checker.
- `style.css`: CSS file for styling the application interface.
- `script.js`: JavaScript file for handling the palindrome checking logic.

## Example

Here’s a simple example of the JavaScript code used to check for palindromes:

```javascript
// Example of palindrome checking logic
document.getElementById('checkButton').addEventListener('click', function() {
  const inputString = document.getElementById('inputString').value;
  const result = isPalindrome(inputString);
  
  document.getElementById('result').textContent = result ? 'The string is a palindrome.' : 'The string is not a palindrome.';
});

function isPalindrome(str) {
  const cleanedStr = str.replace(/[^A-Za-z0-9]/g, '').toLowerCase();
  const reversedStr = cleanedStr.split('').reverse().join('');
  return cleanedStr === reversedStr;
}
```

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to submit a pull request. Please ensure your changes align with the project goals and maintain code quality.

## License

This project is licensed under the MIT License – see the [LICENSE.md](LICENSE.md) file for details.
