
# Forms and JS Events

# Forms:

![](https://i2.wp.com/www.tutorialbrain.com/wp-content/uploads/2019/01/HTML-Form.jpg?fit=1920%2C1080&ssl=1)

### An HTML form is used to collect user input. The user input is most often sent to a server for processing.
### The HTML `<form>` element is used to create an HTML form for user input:

#### Example:
```
    <form>
    .
    form elements
    .
    </form>
```

### The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

## The `<input>` Element:

### The HTML `<input>` element is the most used form element.

### An `<input>` element can be displayed in many ways, depending on the type attribute.

| Type | Description |
| ---- | ----------- | 
| <input type="text"> | Displays a single-line text input field | 
| <input type="radio"> | Displays a radio button (for selecting one of many choices) | 
| <input type="checkbox"> | Displays a checkbox (for selecting zero or more of many choices) | 
| <input type="submit"> | Displays a submit button (for submitting the form) | 
| <input type="button">	| Displays a clickable button |

## Radio Buttons

#### The `<input type="radio">` defines a radio button.

#### Radio buttons let a user select ONE of a limited number of choices.

### Example:
```
    <form>
        <input type="radio" >
    </form>
```

## Checkboxes

#### The `<input type="checkbox">` defines a checkbox.

#### Checkboxes let a user select ZERO or MORE options of a limited number of choices.

### Example
```
    <form>
        <input type="checkbox">
    </form>
```

## The Submit Button

#### The `<input type="submit">` defines a button for submitting the form data to a form-handler.

#### The form-handler is typically a file on the server with a script for processing input data.

#### The form-handler is specified in the form's action attribute.

### Example:
```
    <form action="/action_page.php">
        <input type="text">
        <input type="submit" value="Submit">
    </form>
```

## The Name Attribute for `<input>`

#### Notice that each input field must have a name attribute to be submitted.

#### If the name attribute is omitted, the value of the input field will not be sent at all.

## Lists:

| Value | Description |
| ----- | ----------- | 
|disc |	Default value. The marker is a filled circle |	
|armenian | The marker is traditional Armenian numbering |	
|circle | The marker is a circle |
|cjk-ideographic | The marker is plain ideographic numbers	|
|decimal | The marker is a number |
|decimal-leading-zero | The marker is a number with leading zeros (01, 02, 03, etc.) |
|georgian | The marker is traditional Georgian numbering |	
|hebrew | The marker is traditional Hebrew numbering	|
|hiragan |	The marker is traditional Hiragana numbering |
|hiragana-iroha | The marker is traditional Hiragana iroha numbering |	
|katakana | The marker is traditional Katakana numbering |	
|katakana-iroha | The marker is traditional Katakana iroha numbering |	
|lower-alpha | The marker is lower-alpha (a, b, c, d, e, etc.)	|
|lower-greek | The marker is lower-greek |
|lower-latin | The marker is lower-latin (a, b, c, d, e, etc.)	|
|lower-roman | The marker is lower-roman (i, ii, iii, iv, v, etc.) |	
|none | No marker is shown |
|square | The marker is a square |	
|upper-alpha | The marker is upper-alpha (A, B, C, D, E, etc.) |
|upper-greek | The marker is upper-greek |
|upper-latin | The marker is upper-latin (A, B, C, D, E, etc.)	|
|upper-roman | The marker is upper-roman (I, II, III, IV, V, etc.) |	
|initial | Sets this property to its default value. Read about initial |	
|inherit | Inherits this property from its parent element. Read about inherit |

## list-style-image

### Example
```
    ul {
    list-style-image: url('sqpurple.gif');
    }
```

## list-style-position:

### outside
#### The marker sits to the left of the block of text. (This is the default behaviour if this property is not used.)

### inside
#### The marker sits inside the box of text (which is indented).

## Table Properties:

`width` to set the width of the table
`padding` to set the space between the border of each table cell and its content
`text-transform` to convert the content of the table headers to uppercase 
`letter-spacing`,`font-size` to add additional styling to the content of the table headers
`border-top`, `border-bottom` to set borders above and below the table headers
`text-align` to align the writing to the left of some table cells and to the right of the others
`background-color` to change the background color of the alternating table rows
`:hover` to highlight a table row when a user's mouse goes over it

## Event JS:

![](https://res.cloudinary.com/practicaldev/image/fetch/s--ykbIB8fj--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/7oc46hryju4lpptf954u.jpg)

#### To assign events to HTML elements you can use event attributes.

### Example:
```
    <script>
        document.getElementById("myBtn").onclick = displayDate;
    </script>
```

### The onload and onunload Events
##### The `onload` and onunload events are triggered when the user enters or leaves the page.

##### The `onload` event can be used to check the visitor's browser type and browser version, and load the proper version of the web page based on the information.

##### The `onload` and onunload events can be used to deal with cookies.

### Example
```
<body onload="checkCookies()">
```

### The onchange Event
##### The onchange event is often used in combination with validation of input fields.
