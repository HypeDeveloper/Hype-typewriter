# Typist

Typist is a JavaScript class that provides a typewriter effect. It simulates the typing and deleting of text, creating a typewriter-like animation. This can be useful for adding an engaging and interactive element to your web pages.

## Usage

To use the Typist class, follow these steps:

1. Create an instance of the Typist class, passing the desired options as an argument.

   ```javascript
   const typist = new Typist(options);
   
   
 The options parameter is an object that can contain the following properties:

targetId (string): The ID of the HTML element where the typewriter effect will be applied.
typeSpeed (number): The speed at which characters are typed in milliseconds.
delSpeed (number): The speed at which characters are deleted in milliseconds.
cursorClass (string): A CSS class to style the cursor element.
loop (boolean): Whether to restart the typewriter effect after completion.
cursorString (string): The string representing the cursor.
onEnd (function): A callback function to be called when the typewriter effect completes.
Call the start() method to start the typewriter effect.

```javascript
typist.start();


The options parameter is an object that can contain the following properties:

-targetId (string): The ID of the HTML element where the typewriter effect will be applied.
-typeSpeed (number): The speed at which characters are typed in milliseconds.
-delSpeed (number): The speed at which characters are deleted in milliseconds.
-cursorClass (string): A CSS class to style the cursor element.
-loop (boolean): Whether to restart the typewriter effect after completion.
-cursorString (string): The string representing the cursor.
-onEnd (function): A callback function to be called when the typewriter effect completes.
-Call the start() method to start the typewriter effect.

```javascript
typist.start();
This will begin the typewriter animation on the specified target element.

**(Optional)** Control the visibility of the cursor using the hideCursor() and showCursor() methods.

```javascript
typist.hideCursor(); // Hide the cursor
typist.showCursor(); // Show the cursor
These methods allow you to hide or show the blinking cursor element associated with the typewriter effect.

Ensure that you have an HTML element with the specified targetId where the typewriter effect will be applied.

```html
<div id="typist-container"></div>
Make sure to replace "typist-container" with the actual ID of your target element.

###Examples
Here's an example of using the Typist class with some sample options:

```javascript
const typist = new Typist({
  targetId: 'typist-container',
  typeSpeed: 150,
  delSpeed: 800,
  cursorClass: 'custom-cursor',
  loop: true,
  cursorString: '|',
  onEnd: () => {
    console.log('Typewriter effect completed');
  },
});

typist.start();
In this example, the typewriter effect will be applied to an element with the ID "typist-container". The characters will be typed at a speed of 150 milliseconds, deleted at a speed of 800 milliseconds, and a custom CSS class named "custom-cursor" will be applied to the cursor element. The effect will loop indefinitely, and the cursor will be displayed as a vertical bar (|). Finally, the onEnd callback function will be executed when the typewriter effect completes.

###License
This project is licensed under the MIT License.
