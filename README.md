# Palindrome-Checker-project
# Palindrome-Checker-project.
# Project Title 🚀

## Project Description 📝

> Provide a detailed overview of your project. Explain what it does, why it is useful, and any other relevant information.

Examples;
Iwork index.html styles.css script.js

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
    <title>Palindrome Checker</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <main class="container">
        <h1 class="title">Fatima Palindrome Checker Project</h1>
      <h1 class="title">Is it a Palindrome?</h1>
      <div class="palindrome-div">
        <label for="text-input"
          >Enter in text to check for a palindrome:
        </label>
        <input class="palindrome-input" id="text-input" value="" type="text" />
        <button class="palindrome-btn" id="check-btn">Check</button>
        <div class="results-div hidden" id="result"></div>
      </div>
      <div class="palindrome-definition-div">
        <p class="palindrome-definition">
          <span role="img" aria-label="light-bulb">&#128261;</span>
          A <dfn>palindrome</dfn> is a word or sentence that's spelled the same
          way both forward and backward, ignoring punctuation, case, and
          spacing.
        </p>
      </div>
    </main>
    <script src="script.js"></script>
  </body>
</html>

```css
/* You can also include CSS code snippets. */
```
body {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  background-color: #5ec5e4;
  color: #fff;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  width: 100%;
  min-height: 100vh;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.title {
  text-align: center;
  padding: 10px 0;
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.palindrome-div {
  width: 450px;
  min-height: 100px;
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  padding: 20px;
  margin: 10px 0;
  background-color: white;
  box-shadow: 0 6px 6px #7b184a;
}

.palindrome-definition-div {
  width: 450px;
  font-size: 1.3rem;
  min-height: 140px;
  background-color: #360047;
  margin-top: 20px;
  padding: 20px;
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
}

label {
  color: #0a0a23;
  margin-bottom: 20px;
}

.palindrome-input {
  height: 30px;
  width: 250px;
  text-align: center;
  font-size: 1.2rem;
  margin: 10px;
  border: none;
  border-bottom: 2px solid #5a01a7;
}

.palindrome-btn {
  width: 90px;
  border: none;
  padding: 10px;
  border-radius: 15px;
  background-color: #0cc631;
  color: #fff;
  cursor: pointer;
}

.results-div {
  overflow-y: auto;
  word-wrap: break-word;
  min-height: 50px;
  color: black;
}

.user-input {
  font-size: 1.4rem;
  margin-top: 10px;
  text-align: center;
}

.palindrome-definition {
  vertical-align: middle;
  text-align: center;
}

```javascript
// You can also include JavaScript code snippets.
```
const userInput = document.getElementById('text-input');
const checkPalindromeBtn = document.getElementById('check-btn');
const resultDiv = document.getElementById('result');

const checkForPalindrome = (input) => {
  const originalInput = input; // Store for later output

  if (input === '') {
    alert('Please input a value');
    return;
  }

  // Remove the previous result
  resultDiv.replaceChildren();

  const lowerCaseStr = input.replace(/[^A-Za-z0-9]/gi, '').toLowerCase();
  const resultMsg = `<strong>${originalInput}</strong> ${
    lowerCaseStr === [...lowerCaseStr].reverse().join('') ? 'is' : 'is not'
  } a palindrome.`;

  const pTag = document.createElement('p');
  pTag.className = 'user-input';
  pTag.innerHTML = resultMsg;
  resultDiv.appendChild(pTag);

  // Show the result.
  resultDiv.classList.remove('hidden');
};

checkPalindromeBtn.addEventListener('click', () => {
  checkForPalindrome(userInput.value);
  userInput.value = '';
});

userInput.addEventListener('keydown', (e) => {
  if (e.key === 'Enter') {
    checkForPalindrome(userInput.value);
    userInput.value = '';
  }
});

## Demo 📸

Include a demo or animated GIF of your project. You can use tools like [asciinema](https://asciinema.org/) to record your terminal sessions.

![Demo]()

## Technologies Used 🛠️

List the technologies or tools you used to develop your project. You can also include the libraries or frameworks you used.

Examples:

- HTML
- CSS
- JavaScript



## Installation 💻

Folow these steps to set up the project on your local machine Ensure you have the following software installed on your machine

git clone 

https://github.com/fatiabdulahi/Palindrome-Checker-project/

## Usage 🎯

you can access to my project through git clone -git clone the HTTP or My SSH code link from the repository you wat to clone

# git clone

## Features ⭐
-javascript

-github usage
-palindrome checker project


## Author 👩‍💻 FATIMA ABDULLAHI

Provide your name and a link to your Social Media profiles. You can also include your email address.


- LinkedIn:https://www.linkedin.com/in/fatima-abdullahi-6288662b2
- Email: fatima333abdullahi@gmail.com

## Contributing 🤝

Provide guidelines for others who want to contribute to your project. Include information on how to submit bug reports, feature requests, or pull requests.

## License 📜

Specify the license under which your project is distributed. Include any relevant copyright or attribution notices.
We welcome contributions from the community! Please follow the guidelines below to contribute to our project.
1: Fork the Repository: Click the "Fork" button at the top right of the repository page to create a copy of the repository on your GitHub account.
2: Clone Your Fork: Clone your forked repository to your local machine using the following command:git clone https://github.com/yourusername/yourprojectname.git
3: Create a Branch: Create a new branch for your work to ensure your changes are isolated from the main branch:git checkout -b feature-or-bugfix-description
4: Make Your Changes: Implement your changes, whether fixing a bug or adding a new feature. Be sure to follow the project's coding standards and guidelines.
5: Commit Your Changes: Commit your changes with a descriptive commit message:git add . git commit -m "Description of the changes"
6: Push to Your Fork: Push your changes to your forked repository:git push origin feature-or-bugfix-description
7: Submit a Pull Request: Go to the original repository and submit a pull request from your forked repository. Provide a clear and concise description of your changes and why they should be merged.

License 📜