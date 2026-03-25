# JavaScript Events

A JavaScript event is an action or occurrence that happens in the browser, and JavaScript can detect it and respond to it.

| Event       | Meaning                           |
| ----------- | --------------------------------- |
| `click`     | user clicks an element            |
| `dblclick`  | user double-clicks                |
| `mouseover` | mouse moves over element          |
| `mouseout`  | mouse leaves element              |
| `keydown`   | key is pressed down               |
| `keyup`     | key is released                   |
| `input`     | user types in input               |
| `change`    | value changes                     |
| `submit`    | form is submitted                 |
| `focus`     | input gets focus                  |
| `blur`      | input loses focus                 |
| `load`      | page or resource finishes loading |


Mouse Events

A mouse event is triggered when the user click some element, move the mouse pointer over an element, etc. Here're some most important mouse events and their event handler.

1. The Click Event (onclick)

The click event occurs when a user clicks on an element on a web page.

`onclick`

```
<button type="button" onclick="alert('You have clicked a button!');">Click Me</button>
<a href="#" onclick="alert('You have clicked a link!');">Click Me</a>

```

2. The Contextmenu Event (oncontextmenu)

The contextmenu event occurs when a user clicks the right mouse button on an element to open a context menu.

`oncontextmenu`

example:

```
<button type="button" oncontextmenu="alert('You have right-clicked a button!');">Right Click on Me</button>
<a href="#" oncontextmenu="alert('You have right-clicked a link!');">Right Click on Me</a>

```

3. The Mouseover Event (onmouseover)

The mouseover event occurs when a user moves the mouse pointer over an element.

`onmouseover`

example:

```
<button type="button" onmouseover="alert('You have placed mouse pointer over a button!');">Place Mouse Over Me</button>
<a href="#" onmouseover="alert('You have placed mouse pointer over a link!');">Place Mouse Over Me</a>

```

4. The Mouseout Event (onmouseout)

The mouseout event occurs when a user moves the mouse pointer outside of an element.

`onmouseout`

example:

```
<button type="button" onmouseout="alert('You have moved out of the button!');">Place Mouse Inside Me and Move Out</button>
<a href="#" onmouseout="alert('You have moved out of the link!');">Place Mouse Inside Me and Move Out</a>

```

Keyboard Events

A keyboard event is fired when the user press or release a key on the keyboard.

1. The Keydown Event (onkeydown)

The keydown event occurs when the user presses down a key on the keyboard.

`onkeydown`

example:

```
<input type="text" onkeydown="alert('You have pressed a key inside text input!')">
<textarea onkeydown="alert('You have pressed a key inside textarea!')"></textarea>

```

2. The Keyup Event (onkeyup)

The keyup event occurs when the user releases a key on the keyboard.

`onkeyup`

example:

```
<input type="text" onkeyup="alert('You have released a key inside text input!')">
<textarea onkeyup="alert('You have released a key inside textarea!')"></textarea>

```

3. The Keypress Event (onkeypress)

The keypress event occurs when a user presses down a key on the keyboard that has a character value associated with it

Note: keys like Ctrl, Shift, Alt, Esc, Arrow keys, etc. will not generate a keypress event 

`onkeypress`

example:

```
<input type="text" onkeypress="alert('You have pressed a key inside text input!')">
<textarea onkeypress="alert('You have pressed a key inside textarea!')"></textarea>

```

Form Events

A form event is fired when a form control receive or loses focus or when the user modify a form control value such as by typing text in a text input, select any option in a select box etc. 



1. The Focus Event (onfocus)

The focus event occurs when the user gives focus to an element on a web page.

`onfocus`

example:
```
<script>
    function highlightInput(elm){
        elm.style.background = "yellow";
    }    
</script>
<input type="text" onfocus="highlightInput(this)">
<button type="button">Button</button>

```
2. The Blur Event (onblur)

The blur event occurs when the user takes the focus away from a form element or a window.

`onblur`

example:

```
<input type="text" onblur="alert('Text input loses focus!')">
<button type="button">Submit</button>

```

3. The Change Event (onchange)

The change event occurs when a user changes the value of a form element.

`onchange`

example:

```
<select onchange="alert('You have changed the selection!');">
    <option>Select</option>
    <option>Male</option>
    <option>Female</option>
</select>

```

4. The Submit Event (onsubmit)

The submit event only occurs when the user submits a form on a web page.

`onsubmit`

```

<form action="action.php" method="post" onsubmit="alert('Form data will be submitted to the server!');">
    <label>First Name:</label>
    <input type="text" name="first-name" required>
    <input type="submit" value="Submit">
</form>

```

Document/Window Events

Events are also triggered in situations when the page has loaded or when user resize the browser window, etc. 

1. The Load Event (onload)

The load event occurs when a web page has finished loading in the web browser.

`onload`

example:

```

<body onload="window.alert('Page is loaded successfully!');">
    <h1>This is a heading</h1>
    <p>This is paragraph of text.</p>
</body>

```

2. The Unload Event (onunload)

The unload event occurs when a user leaves the current web page.

`onunload`

example:

```
<body onunload="alert('Are you sure you want to leave this page?');">
    <h1>This is a heading</h1>
    <p>This is paragraph of text.</p>
</body>

```

3. The Resize Event (onresize)

The resize event occurs when a user resizes the browser window. The resize event also occurs in situations when the browser window is minimized or maximized.

`onresize`

example:

```
<p id="result"></p>
<script>
    function displayWindowSize() {
        let w = window.outerWidth;
        let h = window.outerHeight;
        let txt = "Window size: width=" + w + ", height=" + h;
        document.getElementById("result").innerHTML = txt;
    }
    window.onresize = displayWindowSize;
</script>

```