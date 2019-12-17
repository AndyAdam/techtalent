# JAVASCRIPT FUNDAMENTALS

#### Searching for JavaScript:

**W3Schools:** => Google for: `w3schools js alert`, `w3schools js String`, etc.

**MDN JS:** => Google for: `mdn js alert`, `mdn js String`, etc.

<details>

<summary>JavaScript Day 01</summary>

### What can you build with JavaScript?

- [Dynamic HTML Pages](https://www.w3schools.com/js/)
- Web Applications:
  - [Photopea: A Photoshop Clone](https://www.photopea.com/)
- Desktop Applications (Using [Electron.JS](https://electronjs.org/))
  - [Skype](https://www.skype.com/en/)
  - [Slack](https://slack.com/)
  - [Visual Studio Code](https://code.visualstudio.com/)
- [Bookmarklets](https://en.wikipedia.org/wiki/Bookmarklet)
- [Browser Extensions](https://en.wikipedia.org/wiki/Browser_extension)
- [Mobile Apps](https://facebook.github.io/react-native/)
- [Server Applications](https://nodejs.org/en/)
- [Command Line Tools](https://developer.atlassian.com/blog/2015/11/scripting-with-node/)
- [Electronics (Arduino)](https://www.espruino.com/)
- [Artificial Intelligence / Machine Learning](https://js.tensorflow.org/)
- [Brain Controlled Applications!](https://www.youtube.com/watch?v=7KhFO-qCVyg)  


### CODE

- Hello World
  - [hello.html](./code/hello.html)
  - [hello.js](./code/hello.js)
- [Strings](./code/strings.html)
- [Numbers](./code/numbers.html)
- [typeof Operator](./code/typeof.html)

### QUESTIONS

**_How do we clear the console?_**

- Click the `Clear Console` Button
- Press `Ctrl + L`
- Write `console.clear();`

**_How do we change the default browser used by the Live Server VSCode extension?_**

- Go to `File > Preferences > Settings` and search for `Live Server custom browser`
- In the `Live Server: Custom Browser` setting select your favorite Browser
- Note: Settings are saved automatically
- Note: On Mac you can access the Settings from: `Code > Preferences > Settings`

</details>

<details>

<summary>JavaScript Day 02</summary>

### CODE

- [Arrays](./code/arrays.html)

### QUESTIONS

**_What happens if I omit the ; after a statement? Is it optional?_**

- If you omit a semicolon `;` at the end of the statement, JavaScript will try to guess and automatically place the semicolon itself. Most of the times, it does a good job at this, but there are cases where the automatic semicolon placement mechanism will produce undesirable effects. Therefore, we tend to place the semicolons ourselves. Try to get into the habit of placing semicolons at the end of your statements.

**_Does the semicolons at the end of JavaScript statements work much like the ones in CSS?_**

- In a way, they do. Just like we must end each CSS rule with a semicolon; we also have to end each JS statement with a semicolon too, but, unlike CSS, JavaScript can deal with omitted semicolons by placing them automatically. So, most of the time, our statements will work without semicolons at the end, whereas in CSS an omitted semicolon will break subsequent CSS rules.

**_Are the `break` and `default` statements optional inside the `switch` statement?_**

- Yes, they can be omitted, but make sure to check out the following 2 MDN resources:
- [_What happens if I forgot a break?_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch#What_happens_if_I_forgot_a_break)
- [`Switch` description](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch#Description)

**_When we do a string comparison with ==, e.g. "4" == 3, which operand gets converted?_**

- _The String part is converted to a Number, e.g. "4" becomes 4 and then it's value is compared with 3_
  <br/>
  (Reference: [Comparing Strings to Numbers](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20%26%20grammar/ch4.md#comparing-strings-to-numbers))

**_How does the switch statement compares the switch value with each case value?_**

Example:

```
switch (a) {
	case 2:
		// do something
		break;
	case 42:
		// do another thing
		break;
	default:
		// fallback to here
}
```

- _"...the matching that occurs between the **a** expression and each case expression is identical to the === algorithm."_
  Reference: [](https://github.com/getify/You-Dont-Know-JS/blob/f0d591b6502c080b92e18fc470432af8144db610/types%20%26%20grammar/ch5.md#switch)

- **_How do we print newlines to the console?_**

Using the '\n' escape character.

`console.log("A line and \n another line and yet \n another line!");`

- **_When should we place the &lt;script&gt; tags in the &lt;head&gt; area?_**

  - When you insert a library script such as the jQuery library
  - When performance/page load times are not considerably affected by the script
  - When you want to tweak CSS styling before the body is rendered via a script.

### VISUALIZATIONS

- _Arrays:_ [Dynamic relationship with variables and values.](http://www.pythontutor.com/javascript.html#code=const%20numbers%20%3D%20%5B%200,%201,%202,%203%20%5D%3B%0Alet%20names%20%3D%20%5B%20%22Kostas%22,%20%22Chris%22,%20%22Abdul%22%20%5D%3B%0Alet%20mixed%20%3D%20%5B%20123,%20true,%20%22TEXT%22,%20%5B%201,2,3,4%5D%20%5D%3B%0A%0Aconsole.log%28%20numbers%20%29%3B%0A%0Aconsole.log%28%20typeof%20numbers%20%29%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
- _Arrays:_ [push, pop, shift, unshift & length.](https://goo.gl/K28s5m)
- _Arrays:_ [Change the value of a specific Array element.](https://goo.gl/TkmdNj)
- _Arrays:_ [Different behaviors with const and array values](https://goo.gl/Diurj7)

### REFERENCES

- [What is the difference between placing &lt;script&gt; in head and before &lt;/body&gt;?](https://www.reddit.com/r/javascript/comments/5di1va/what_is_the_difference_between_placing_script_in/)
- [The `defer` and `async` script attributes](https://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)
- [Where to place JavaScript in an HTML file?](https://stackoverflow.com/questions/196702/where-to-place-javascript-in-an-html-file)
- [String Methods](https://www.w3schools.com/js/js_string_methods.asp)
- [Number Methods](https://www.w3schools.com/js/js_number_methods.asp)
- [Array Methods - Full Reference](https://www.w3schools.com/js/js_array_methods.asp)
  - [Array push()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
  - [Array pop()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)
  - [Array shift()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift)
  - [Array.unshift()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift)
- [Should I write script in the body or the head of the html? [duplicate]](https://stackoverflow.com/questions/3531314/should-i-write-script-in-the-body-or-the-head-of-the-html)
- [When to use the &lt;script&gt; tag in the head and body section of a html page? ](https://stackoverflow.com/questions/38407962/when-to-use-the-script-tag-in-the-head-and-body-section-of-a-html-page?noredirect=1&lq=1)
- [Loose Equals == vs. Strict Equals ===](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20%26%20grammar/ch4.md#loose-equals-vs-strict-equals)
- [The Switch Statement](https://github.com/getify/You-Dont-Know-JS/blob/f0d591b6502c080b92e18fc470432af8144db610/types%20%26%20grammar/ch5.md#switch)

</details>

<details>

<summary>JavaScript Day 03</summary>

### CODE

- [Array Loops](./code/array-loop.html)
- [Functions](./code/functions.html)
- Quick Array Reference:

      	`let months = [ 1, 2, 3 ];`<br/>
      	`months.push( 4, 5, 6 ); 	// [ 1, 2, 3, `**`4, 5, 6`**` ]`<br/>
      	`months.pop();      		// [ 1, 2, 3, 4, 5 ]`<br/>
      	`months.shift();    		// [ 2, 3, 4, 5 ]`<br/>
      	`months.unshift( 0, 1 ); 	// [ `**`0, 1`**`, 2, 3, 4, 5]`<br/>
      	`months[0]; 				// 0`<br/>
      	`months[1]; 				// 1`<br/>

      	**NESTED ARRAYS:** Arrays inside Arrays and how to access them
      	```
      	let nested = [
      1,
      2,
      3,
      [ "Corto", "Maltese" ]

  ];
  ```
  `nested[0]; // 1`<br/>
  `nested[1]; // 2`<br/>
  `nested[2]; // 3`<br/>
  `nested[3]; // [ "Corto", "Maltese" ]`<br/>
  `nested[3][0]; // "Corto"`<br/>
  `nested[3][1]; // "Maltese"`<br/>

### QUESTIONS

**_Can we manually break out of an Infinite Loop?_**

- If you're using Chrome, `Shift-Esc` to bring up the Chrome task manager, and kill the task.<br/>Reference: [TeamTreehouse](https://teamtreehouse.com/community/i-have-an-infinite-loop-in-a-tab-i-cant-close) / [Stack Overflow](https://stackoverflow.com/questions/905322/how-do-you-stop-an-infinite-loop-in-javascript)

### REFERENCES

- [How to avoid infinite loops in JavaScript](https://www.dummies.com/web-design-development/avoid-infinite-loops-javascript/)
- [Visualization of passing data **by Value** vs. **by Reference**](http://www.pythontutor.com/visualize.html#code=let%20fruit%20%3D%20%22apple%22%3B%0Alet%20fruit2%20%3D%20fruit%3B%0A%0Aconsole.log%28%20%22%5Cnfruit%3A%22,%20fruit%20%29%3B%0Aconsole.log%28%20%22fruit2%3A%22,%20fruit2%20%29%3B%0A%0Afruit%20%3D%20%22orange%22%3B%0A%0Aconsole.log%28%20%22%5Cnfruit%3A%22,%20fruit%20%29%3B%0Aconsole.log%28%20%22fruit2%3A%22,%20fruit2%20%29%3B%0A%0Alet%20fruitBasket%20%3D%20%5B%20%22apples%22%20,%20%22oranges%22%20%5D%3B%0Alet%20fruitBasket2%20%3D%20fruitBasket%3B%0A%0Aconsole.log%28%20%22%5CnfruitBasket%3A%22,%20fruitBasket%20%29%3B%0Aconsole.log%28%20%22fruitBasket2%3A%22,%20fruitBasket2%20%29%3B%0A%0AfruitBasket%5B0%5D%20%3D%20%22bananas%22%3B%0A%0Aconsole.log%28%20%22%5CnfruitBasket%3A%22,%20fruitBasket%20%29%3B%0Aconsole.log%28%20%22fruitBasket2%3A%22,%20fruitBasket2%20%29%3B%0A%0Alet%20person%20%3D%20%7B%20name%3A%20%22John%22%20%7D%0Alet%20anotherPerson%20%3D%20person%3B%0AanotherPerson.name%20%3D%20%22Jane%22%3B%0A%0Aconsole.log%28%20%22%5CanotherPerson%3A%22,%20anotherPerson%20%29%3B%0Aconsole.log%28%20%22person%3A%22,%20person%20%29%3B&cumulative=false&curInstr=18&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)
- _( See Resources - Tools section below for the Chrome Extension that displays a warning icon at the bottom right section of the webpage to indicate JavaScript errors on web pages. Here's a [video](https://www.youtube.com/watch?v=jh07STUs7Ok) showing how to install and use the Extension.)_

</details>

### RESOURCES | TOOLS

- [JavaScript Errors Notifier Extension for Chrome](https://chrome.google.com/webstore/detail/javascript-errors-notifie/jafmfknfnkoekkdocjiaipcnmkklaajd?hl=en)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Live Server extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Python Tutor Visualizations in JavaScript](http://www.pythontutor.com/javascript.html#mode=edit)

### RESOURCES | LEARNING

- [SoloLearn JavaScript Tutorial](https://www.sololearn.com/Course/JavaScript/)
- [You Don't Know JS](https://github.com/getify/You-Dont-Know-JS)
- [JavaScript Tutorial](http://www.javascripttutorial.net/)
- [The JavaScript Handbook, by Flavio Copes](https://flaviocopes.com/page/ebooks/)
- [JavaScript 30 - Build 30 things in 30 days with 30 tutorials](https://javascript30.com/)
- [Introduction to JavaScript](https://scrimba.com/g/gintrotojavascript)
- [JavaScript Tutorial: Learn JavaScript in 1 Hour [2019]](https://www.youtube.com/watch?v=W6NZfCO5SIk)
- [FreeCodeCamp](https://www.freecodecamp.org/)
- [JavaScript Phrasebook](https://www.amazon.com/JavaScript-Phrasebook-Christian-Wenz/dp/0672328801)
