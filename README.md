#Password Generator:
A simple and clean web-based password generator built with vanilla HTML, CSS, and JavaScript. It allows users to create strong, random passwords based on customizable criteria like length and character types.

Link : 

ScreenShort : 

#Features : 
. Customizable Password Length: Adjust the password length from 1 to 30 characters using an intuitive slider.

. Character Set Options: Choose to include or exclude specific character types:

  . Uppercase Letters (A-Z)

  . Lowercase Letters (a-z)

  . Numbers (0-9)

  . Symbols (~!@#$%^&*)

. One-Click Copy: Easily copy the generated password to your clipboard with a single click on the copy icon.

. User Feedback: The copy icon changes to a checkmark for 3 seconds to confirm that the password has been copied.

. Clean UI: A modern and straightforward user interface with a pleasant gradient background.

#Technologies Used : 
1. HTML5: For the basic structure and content of the web page.

2. CSS3: For styling the components, layout, and visual effects.

3. JavaScript (ES6): For the core functionality, including password generation logic, DOM manipulation, and event handling.

# How to Use : 
To run this project locally, follow these simple steps:

1. Clone the repository: git clone https://github.com/your-username/your-repo-name.git
   
2. Navigate to the project directory: cd your-repo-name

3. Open the index.html file in your web browser.

* That's it! You can now generate passwords.

#Code Overview : 
script.js

This file contains all the logic for the application.

  . DOM Element Selection: All required HTML elements (slider, buttons, checkboxes, etc.) are selected at the beginning.

  . Event Listeners:

     . An input event listener on the slider updates the "Password Length" display in real-time.

     . A click event listener on the "Generate Password" button triggers the generatePassword() function.

     . A click event listener on the copy icon uses the navigator.clipboard.writeText() API to copy the password from the display box.

  . generatePassword() Function:

     1. Initializes an empty string allChars which will hold the pool of characters to choose from.

     2. Checks which checkboxes are ticked and concatenates the corresponding character sets (lowerChars, upperChars, etc.) to allChars.

     3. If no character sets are selected, it returns an empty string.

     4. It then loops for a number of times equal to the selected password length, each time picking a random character from allChars and appending it to the final genPassword string.

