Read: 05 - Design web pages with CSS

CSS (Cascading Style Sheets) allows you to create great-looking web pages
Using CSS you can control exactly how HTML elements look in the browser, presenting your markup using whatever design you like.

Note: A browser is sometimes called a user agent, which basically means a computer program that represents a person inside a computer system. Browsers are the main type of user agent we think of when talking about CSS, however, it is not the only one. There are other user agents available — such as those which convert HTML and CSS documents into PDFs to be printed.

CSS Syntax :
CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text."

h1 {
    color: red;
    font-size: 5em;
}


Three Ways to Insert CSS
There are three ways of inserting a style sheet:

External CSS
Internal CSS
Inline CSS


For external :
External styles are defined within the <link> element, inside the <head> section of an HTML page:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>


Here is how the "mystyle.css" file looks:

"mystyle.css"
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}


Note: Do not add a space between the property value and the unit (such as margin-left: 20 px;). The correct way is: margin-left: 20px;


Internal CSS
An internal style sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the <style> element, inside the head section.

Example
Internal styles are defined within the <style> element, inside the <head> section of an HTML page:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
Inline CSS
An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

Example
Inline styles are defined within the "style" attribute of the relevant element:

<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
Tip: An inline style loses many of the advantages of a style sheet (by mixing content with presentation). Use this method sparingly.

Multiple Style Sheets
If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used. 

Assume that an external style sheet has the following style for the <h1> element:

h1 {
  color: navy;
}
Then, assume that an internal style sheet also has the following style for the <h1> element:

h1 {
  color: orange;   
}
Example
If the internal style is defined after the link to the external style sheet, the <h1> elements will be "orange":

<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
  color: orange;
}
</style>
</head>
Example
However, if the internal style is defined before the link to the external style sheet, the <h1> elements will be "navy": 

<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
Cascading Order
What style will be used when there is more than one style specified for an HTML element?

All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

Inline style (inside an HTML element)
External and internal style sheets (in the head section)
Browser default
So, an inline style has the highest priority, and will override external and internal styles and browser defaults.


CSS color Property

Example
Set the text-color for different elements:

body {
  color: red;
}

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}
More "Try it Yourself" examples below.

Definition and Usage
The color property specifies the color of text.

Tip: Use a background color combined with a text color that makes the text easy to read.

Default value:	not specified
Inherited:	yes
Animatable:	yes. Read about animatable
Version:	CSS1
JavaScript syntax:	object.style.color="#0000FF"




for more information please visit the below links:

-[CSS Tutorial](https://www.w3schools.com/cssref/pr_text_color.asp)

-[CSS Tutorial](-[CSS Tutorial](https://www.w3schools.com/cssref/pr_text_color.asp)

)
