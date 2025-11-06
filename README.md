# css-from-scratch

CSS (Cascading Style Sheets) is used in web development primarily for styling and laying out web pages. Its purpose is to separate the presentation of a document from its content, which is typically structured using HTML.

 Why we need css?
->Separation of Concerns: CSS allows developers to keep the content (HTML) and the styling (CSS) in separate files. This separation improves code organization, making it easier to manage, update, and maintain websites.
->Visual Presentation: CSS defines how HTML elements are displayed on a screen, paper, or other media. This includes properties like: 
->Colors and backgrounds: Setting text colors, background colors, and background images.
->Typography: Controlling fonts, font sizes, weights, and text alignment.
->Layout and positioning: Arranging elements on the page, creating columns, defining margins, padding, and positioning elements precisely.
->Visual effects: Adding borders, shadows, transitions, animations, and other decorative features.

inline
-------------

--> <p style="color: rgb(194, 25, 25);">This paragraph is styled using inline css styling</p>

--> inernal styling 
-----------------------
<html>
  <head>
    <style>
      html{
        color:red;
      }
    </style>
  </head>
</html>

The above code shows how to style using inline css code 


External styling
-------------------
 If we need to use external styiling we need to create a external css file and import the properties using the given code

 <html>
  <head>
    <link rel="stylesheet" href="./style.css" />
  </head>
</html>

the entire css code will be structured in the style.css file 


css selectors
---------------
In CSS, a selector is a pattern used to "find" or select the HTML elements on a web page that you want to style. It is the first part of a CSS rule, which tells the browser which specific elements should have the declared CSS property values applied to them. 

example code :
    h1{
  color: blue;
}

 here the h1 is the selected element 

 class selector
 ------------------
 exaple code:

 .red-text{
    color:red;
 }

 html code for the above class

 <h1 class="red-text">red text</h1>

 id selector
 -----------
 example code:

 #main{
  color:red;
 }

 html code:
  <h2 id="main">red</h2>
  id's are unique . The CSS ID selector is a fundamental tool for applying styles to a specific, unique HTML element within a document.


  Attribute selector
  --------------------
  CSS attribute selectors allow you to select and style HTML elements based on the presence, value, or specific characteristics of their attributes. They provide a powerful way to target elements without relying solely on classes or IDs, especially useful for dynamic content or when attributes carry semantic meaning. 

  example code:
   p[draggable]{
    color:red;
   }

   html code:
   <p draggable="true">drag me</p>

   universal selector
   -------------------
   The universal selector in CSS is a selector that targets all elements within an HTML document. It is denoted by an asterisk (*).

   
    exaple code

    *{
      color:red;
    }


--> font properties
----------------------

h1{
  font-size: 20px;
  font-size: 20pt;
}
/*we acn write font size in pixels and points  likw px and pt*/

/* em and rem */
/* em means 100% of the parent font size 1em means 1xparent font size 2 em means 2xparent font size and In CSS, rem stands for "root em" and is a relative unit of measurement. It is relative to the font size of the root element, which is typically the <html> tag in an HTML document.  */

/* font weight */

/* normal , bold is keywords

lighter , bolder  relative to parent 

number 100-200 */

/* font family */
