🎈 Canvas Balloon Generator

This project is a JavaScript program, originally written for the CodeHS environment, designed to draw a specified number of randomly sized and colored balloons on a canvas, complete with trailing strings.

It demonstrates functions for user input validation, coordinate calculation, and color generation (HSL to Hex conversion).

🚀 Key Features

Custom Input: The application prompts the user for three parameters to customize the scene:

The number of balloons to draw.

A minimum balloon radius.

A maximum balloon radius.

Input Validation: Automatically ensures the minimum and maximum radii are within logical bounds (0-40) and are correctly ordered.

Randomized Aesthetics: Each balloon is drawn with a random, bright color and a random radius within the specified range.

String Drawing: The balloons are connected by a string line starting from the bottom of the canvas.

⚠️ Execution Warning (CodeHS Dependencies)

This code relies on several CodeHS-specific global functions and objects which are not available in a standard web browser environment (like running a simple index.html file):

readInt(): Used for user input. In a browser, this would typically be replaced by prompt() or a form input field.

removeAll(): Used to clear the canvas. In standard Canvas, this requires ctx.clearRect().

getWidth(), getHeight(): Used to get canvas dimensions. In standard Canvas, these are properties of the canvas element (e.g., canvas.width).

Line(), Circle(), add(): These are custom graphics objects/methods specific to the CodeHS library. To run this code, you must replace these calls with native Canvas 2D Context (ctx) drawing commands (ctx.beginPath(), ctx.arc(), ctx.lineTo(), ctx.stroke(), etc.).

💡 Suggested Browser Adaptations

To make this runnable in a web browser, the main() and createBalloons() functions would need to be re-written to use standard JavaScript and HTML Canvas commands.

The core logic for randomization, validation, and color conversion (randomInt, randomColor, hslToHex, rgbToHex) is standard and reusable.
