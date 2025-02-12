# Chess-Model-Website

A model of a chessboard along with its pieces using HTML, CSS, and JavaScript. **The chess pieces are not programmed to function.**

## Disclaimer

This project contains code sourced from the internet. **I do not claim ownership of the original code.** My contribution is making it easily accessible, organizing the files, and providing a structured guide on how to customize and modify the project.

---

## Step 1: Download the Files

Download the following files:
- `index.html`: The HTML file containing the structure of the chessboard.
- `style.css`: The CSS file containing the styling for the chessboard and pieces.
- `script.js`: The JavaScript file containing functionality for controlling the chessboard.

## Step 2: Add Files to Your Project

Place the downloaded files in your project directory.

## Step 3: Include the Files in Your HTML

In your HTML file (`index.html`), include the CSS and JavaScript files using the `<link>` and `<script>` tags, respectively.

```html
<link rel="stylesheet" href="style.css">
<script src="script.js"></script>
```

## Step 4: Set Up the HTML Structure

Ensure your HTML file contains the necessary structure for the chessboard and controls. You can copy the structure from the provided `index.html` file.

## Step 5: Customize the Chessboard

Open the `style.css` file to customize the appearance of the chessboard, pieces, and controls. You can modify colors, sizes, animations, and other visual aspects to suit your preferences.

## Step 6: Customize the Chessboard Controls

Open the `script.js` file, where you'll find JavaScript code responsible for controlling various aspects of the chessboard. Below are some common customizations you can make:

### 1. Toggle Animations

By default, the chessboard animations are enabled. You can customize this behavior to toggle animations on or off based on user preference. Locate the relevant code block responsible for animation control and modify it as follows:

```javascript
// Locate the code block responsible for animation control
var animationsEnabled = true; // Change to false to disable animations initially

// Function to toggle animations
function toggleAnimations() {
    animationsEnabled = !animationsEnabled; // Toggle animations state
    if (animationsEnabled) {
        // Re-enable animations
        document.documentElement.classList.remove("noanimations");
    } else {
        // Disable animations
        document.documentElement.classList.add("noanimations");
    }
}

// Attach event listener to a control button or element to trigger the toggleAnimations() function
document.getElementById("toggleAnimationsButton").addEventListener("click", toggleAnimations);
```

### 2. Show/Hide Board Borders

You can provide users with the option to show or hide the borders of the chessboard. Modify the code to implement this functionality:

```javascript
// Locate the code block responsible for board border control
var bordersVisible = true; // Change to false to hide borders initially

// Function to toggle board borders
function toggleBoardBorders() {
    bordersVisible = !bordersVisible; // Toggle borders state
    if (bordersVisible) {
        // Show board borders
        document.documentElement.classList.remove("noborders");
    } else {
        // Hide board borders
        document.documentElement.classList.add("noborders");
    }
}

// Attach event listener to a control button or element to trigger the toggleBoardBorders() function
document.getElementById("toggleBordersButton").addEventListener("click", toggleBoardBorders);
```

### 3. Enable/Disable Body Scrolling

You can allow or prevent body scrolling while interacting with the chessboard. Customize the code to implement this feature:

```javascript
// Locate the code block responsible for body scrolling control
var scrollingEnabled = true; // Change to false to disable body scrolling initially

// Function to toggle body scrolling
function toggleBodyScrolling() {
    scrollingEnabled = !scrollingEnabled; // Toggle scrolling state
    if (scrollingEnabled) {
        // Enable body scrolling
        document.documentElement.classList.remove("noscroll");
    } else {
        // Disable body scrolling
        document.documentElement.classList.add("noscroll");
    }
}

// Attach event listener to a control button or element to trigger the toggleBodyScrolling() function
document.getElementById("toggleScrollingButton").addEventListener("click", toggleBodyScrolling);
```

### 4. Additional Customizations

You can further customize the code to add new controls, change control button styles, or implement additional functionalities based on your requirements.

## Step 7: Test and Deploy

Test your chessboard locally by opening the HTML file in a web browser. Ensure all functionalities work as expected. Once satisfied, deploy your project to a web server or GitHub Pages to share it with others.

---
