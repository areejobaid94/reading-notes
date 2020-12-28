# HTML Text:

![](https://www.technologydiving.com/wp-content/uploads/2016/01/Components-of-HTML-Headings-and-Paragraphs-1-e1460625351428.jpg)

## Headings and paragraphs:

1. ### Headings:

#### HTML headings are defined with the `<h1>` to `<h6>` tags.

#### `<h1>` defines the most important heading. `<h6>` defines the least important heading.

### Example:
```
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
```


2. ### paragraphs:

#### The HTML `<p>` element defines a paragraph.

#### A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.

### Example:
```
    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>
```

## Bold & Italic:

![](https://stuyhsdesign.files.wordpress.com/2015/10/bold-italic.png)

##### By enclosing words in the tags `<b>` and `</b>` we can make characters appear bold.

#### By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic.

## Superscript & Subscrip:

![](https://www.wikihow.com/images/thumb/3/3f/Subscript-and-Superscript-Text-in-HTML-Step-2-Version-2.jpg/v4-460px-Subscript-and-Superscript-Text-in-HTML-Step-2-Version-2.jpg.webp)

### The `<sup>` tag defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes, like WWW[1].

### Example:
```
sup {
  vertical-align: super;
  font-size: smaller;
}
```

### The `<sub>` tag defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O.

### Example:
```
sub {
  vertical-align: sub;
  font-size: smaller;
}
```

## White Space:

### The `white-space` property specifies how `white-space` inside an element is handled.

### Example:
```
div{
   white-space: normal|nowrap|pre|pre-line|pre-wrap|initial|inherit;
}
```

## Strong & Emphasis
### min-width, max-width:

#### The `<strong>` tag is used to define text with strong importance. The content inside is typically displayed in bold.

#### The <strong> tag also supports the Global Attributes in HTML.

### Example:
```
<strong>This text is important!</strong>
```

#### The `<em>` tag is used to define emphasized text. The content inside is typically displayed in italic.

#### A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.

### Example:
```
<p>You <em>have</em> to hurry up!</p>

<p>We <em>cannot</em> live like this.</p>
```

## Quotations

### HTML <blockquote> for Quotations

#### The HTML `<blockquote>` element defines a section that is quoted from another source.

#### Browsers usually indent `<blockquote>` elements.

### HTML `<abbr>` for Abbreviations

#### The HTML `<abbr>` tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".

#### Marking abbreviations can give useful information to browsers, translation systems and search-engines.

### Example:
```
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

```

### HTML `<address>` for Contact Information.

#### The HTML `<address>` tag defines the contact information for the author/owner of a document or an article.

#### The contact information can be an email address, URL, physical address, phone number, social media handle, etc.

#### The text in the `<address>` element usually renders in italic, and browsers will always add a line break before and after the `<address>` element.

### Example:
```
<address>
    Written by John Doe.<br>
    Visit us at:<br>
    Example.com<br>
    Box 564, Disneyland<br>
    USA
</address>
```

### HTML `<cite>` for Work Title

#### The HTML <cite> tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.).

#### Note: A person's name is not the title of a work.

#### The text in the <cite> element usually renders in italic.

#### All HTML elements can be considered as boxes. In CSS, the term "box model" is used when talking about design and layout.

### Example:
```
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```

# Introducing CSS

### The selector points to the HTML element you want to style.
### The declaration block contains one or more declarations separated by semicolons.
### Each declaration includes a CSS property name and a value, separated by a colon.

### Example:
```
 color is property and blue is value.
 font size is property and 12px is value.
```

# JS

### Basic JavaScript Instructions

##### A computer program is a list of "instructions" to be "executed" by a computer.

##### In a programming language, these programming instructions are called statements.

A JavaScript program is a list of programming statements.
#### Loops allow statements to be repeated
- The code to be repeated is in the loop body
- One repetition of the body is called an iteration
- Loops are structurally similar to if statements
- The loop control statement(s) are contained in ()s after the keyword
- The loop body is contained in {}s

### JS switch 

#### The switch statement is used to perform different actions based on different conditions.

#### Use the switch statement to select one of many code blocks to be executed.

### Example

```
switch (new Date().getDay()) {
  case 0:
    day = "Sunday";
    break;
  case 1:
    day = "Monday";
    break;
  case 2:
     day = "Tuesday";
    break;
  case 3:
    day = "Wednesday";
    break;
  case 4:
    day = "Thursday";
    break;
  case 5:
    day = "Friday";
    break;
  case 6:
    day = "Saturday";
}
```
