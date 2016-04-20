# Intro to Web Development Part 1 HTML & CSS
### Grand Circus Detroit   
@CarlosRinger

### `Week 1 - 4/12 & 4/14`
### Attributes
- key/value pairs is an important concept in programming
- attributes must be in quotations  
`<div class= "containers">A bunch of stuff</div>`

### Doctype
`<!doctype html>`
- very first element when writing HTML file  
- backwards compatible
- tells the browser how it should render page

### Main HTML Tags
Tag | Description
------- | -----------
`head` | Contains the page title and metadata
`body` | Contains all of the visible content
`title` | Optional tag. This is the name of your page. Nested in the `head`  tag

### Nesting
HTML elements 'nest' inside one another. The element that opens first closes last

### Content Tags
Element | Description
------- | -----------
`div` | defacto container element
`p` | used for copy
`h1 thru h6` | designating titles/subtitles  
`ol` | create a numbered list  
`ul` | create an unordered list  
`li` | list elements

### Links
#### Anchor element
links to other sites on the web (or within your project) are created using this element  
`<a href="http://facebook.com">Facebook</a>`  
`<a href="about.html">About Me</a>`

#### Link element
Unlike the `link` species relationships between the current document and an external resource

### HTML Comments
Ignored by the browser engine. Able to comment on code like any other coding language  

`<!-- Hello, I am a comment. -->`

### Tables
Tables are a way to represent complex information in a grid format
- made of rows and columns  
- tables are compound elements
- don't use tables to style content, thats why we have CSS!

### Folder Structure


### CSS
Cascading Style Sheets  
- individual components of CSS are called rules
- rules made up of two parts
  - one or more selectors
  - one or more declarations  

- CSS syntax
``` css
h1 {
  color: orange;
  text-align: center;
    }
```
- Declaration = Property + Value

``` css
/* This is a CSS comment
          it can be multi-line */
```  
- Declarations must end in a semicolon

### CSS Properties
#### Common CSS Properties
Property | Description
-------- | -----------
`background-color` | background color for an element  
`color` | color of the text of in an element  
`font-family` | typeface for text  
`font-size` | size for text (px,%,em)  
`font-weight` | bold text  
`text-decoration` | used for underline  
`height` | specifies the height of an element  
`weight` | specifies the width of an element

#### Color in CSS
Color is just a property  

Method | Syntax | Description
------ | ------ | -----------
color name | `white` | a list of 140 predefined colors  
hexidecimal | `FF0000` | RGB values in hex 00-FF (0-255)  
RGB | `rgb(255,0,187)` | RGB vales in decimal numbers  
RGBA | `rgba(255,0,187,0.5)` | RGB values with an added alpha (opacity) value

#### CSS Units
Method | Syntax | Description
------ | ------ | -----------
em | `1em` | Scalable unit based on font size  
pixels | `16px` | Fixed number of pixels  
percent | `120%` | Percent value based on font size

### Block elements
-  Appear on a new line of a web page, like paragraphs
- Takes up all horizontal space it can
- Stretches to fill all the space to the left and right within its parent container
- Stack on top of each other by default
- Block element `<div> <p> <ul> <li> <table>`...and just about everything else

### Inline elements
- Rendered without starting a new line
- Appear side to side until reaching edge of parent container then will start new line
- Stack across the page by default
- Inline element `<a> <img>`

### `Week 2 - 4/19 & 4/21`
### CSS Reset
CSS file that sets all the usual suspects to normalized values, giving you a standard place to start from.  

CSS Reset [http://meyerweb.com/eric/tools/css/reset/]
- A CSS reset is just another css file that you inclue in your project. Only requirement is to load it before your project's css file. Whatever comes last wins so a CSS reset file included after a `styles.css` will overwrite any styles that conflict betweeen the two.

```html
<link rel="stylesheet" href="reset.css">
<link rel="stylesheet" href="styles.css">
```

### The Box Model
Every HTML element is in a box, regardless of its visible shape

The total size of an element is a combination of the following
 - Content
 - Padding
 - Border
 - Margin

### Border
- Border is the edge around the element. It has elements of thickness, style, and color
- CSS property and is defined using CSS rules. There are a few different ways to specify its values

```css
p { /* each property specified separately */)
  border-width
}
```

### Padding
Padding is the space between the element and the border. Padding can be specified in `px` or `em`

### Margin
Like padding & border

### Auto Margin
If margin is set to `auto` on an element that has a set width, it will take up as much space as possible. You can use this to center or justify an element left or right. This only works for horizontally centering

```css
p {
  margin: 0 auto;
  width: 300px;
}

p {
  margin-right: auto;
  margin-left: 10px;
  width: 25%;
}
```



<div class="footer">&copy; 2016 Carlos Ringer</div>
