# CSS Notes
Css stands for Cascading Style Sheets.  CSS is used to STYLE a webpage.  Often CSS is used by referencing a .css stylesheet in your html and making changes within the .css file in your repository instead of writing CSS directly into your HTML document.

## Key Concepts
  - to aid in visualization, it helps to imagine an invisible box around each HTML element on your webpage.  You can manipulate these elements by using different CSS inputs.
 - Taylor took INCREDIBLE notes that are much better than anything I could summarize, so I've included them below;
 
### Chapter 10 Summary:
- CSS treats each HTML element as if it asppears inside its own box and uses rules to indicate how that element should look. 
- Rules are made up of selectors.  Selectors specificy the element the rule applies to.  Rules are also made up of declarations.  Declarations indicate what these elements should look like. 
- Different types of selectors allow you to target your rules at different elements. 
- Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties.  For example, the font-family property sets the choice of font, and the value arial specficies Arial as the preferred typeface. 
- CSS rules usually appear in a spearate document, although they may appear within an HTML page. 

### Chapter 10 Notes 
- The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element 
- CSS allows you to create rules that control the way that each individual box - and the contents of that box - is presented. 
- CSS workks by associating rules with HTML elements.  These rules govern how the content of specified elements should be displayed.  A CSS rule contains two parts: a selector and a declaration. 
    * CSS declarations sit inside curly brackets and each is made up of two parts - a property and a value separted by a colon.  You can specificy several properties in one declaration, each separated by a semi-colon. 
    * Properties indicate the aspects of the element you want to change.  For example, color, font, width height, and border. 
    * Values specificy the settings you want to use for the chosen properties.  For example, if you want to specify a color property then the value is the color you want the text in these elements to be. 

#### Using External CSS
- The `<link>` element can be used in an HTML doc to tell the browser where to find the CSS file used to style the page.  It is an empty element - meaning it does not need a closing tag - and it lives inside the `<head>` element. It should use three attributes: 
    1. href - this specifies the path to the CSS file, which is often placed in a folder called css or styles
    1. type - this attribute specifies the type of document being linked to.  The value should be text/css. 
    1. rel - this specifies the relationship between the HTML page and the file it is linked to.  The value should be a stylesheet when linking to a CSS file. 
- An HTML page can use more than one CSS style sheet. To do this it could have a `<link>` element for every CSS file it uses.  For example, some authors use one CSS file to control the presentation - such as fonts and colors - and a second to control the layout 

#### Using Internal CSS 
- You can also include CSS rules within an HTML page by placing them inside a `<style>` element, which usually sits inside the `<head>` element of the page. 
- The `<style>` element should use the type attribute to indiciate that the styles ar especified in CSS.  The value should be text/css. 
- When building a site with more than one page, you should use an external CSS style sheet.  This: 
    1. Allows all pages to use the same style rules - rather than repeating them in each page 
    1. Keeps the content separate from how the page looks 
    1. Means you can change the styles used across all pages by altering just one file - rather than each individual file 

#### CSS Selectors 
- Selectors are case sensitive, so they must match element names and attribute values exactly. 

**Most commonly used CSS Selectors**
- Universal selector  applies to all elemetns in the document 
    * Ex: `* {}`
    * meaning - applies to all elements in the document 
- Type selector  matches eelement names, targers the h1, h2, h3 elements. 
    * Ex: `h1, h2, h3 {}` - this will target the h1, h2, h3 elements 
    * Meaning - matches element names 
- Class Selector 
    * Ex: `.note{}` - targets any element whose class attribute has a value note 
    * Ex: `p.note{}` - targets only `<p>` elements whose class attribute has a value of note 
    * Meaning - matches an element whose class attribute has a value that matches the one specified after the period or full stop symbol 
- ID Selector 
    * Ex: `#introduction {}` - targets the element whose id attributes has a value of introduction
    * Meaning - matches an element whose id attributes has a value that matches the one specified after the pound of hash symbol 
- Child Selector 
    * Ex: `li>a {}` - targets any `<a>` elements that are children of an `<li>` element not not other `<a>` elements in the page 
    * Meaning - matches an element that is a direct child of another 
- Descendant Selector 
    * Ex: `p a {}` - targets any `<a>` elements that sit inside a `<p>` element even if there are other elements nested between them. 
    * Meaning - mathces an element that is a descendent of another specified element, not just a direct child of that element 
- Adjacent Sibling Selector 
    * Ex: `h1+p {}` - targets the first `<p>` element after any h1 element but not other `<p>` elements 
    * Meaning - matches an element that is the next sibling of another 
- General sibling selector 
    * Ex: `h1~p {}` - if you have two `<p>` elements that are siblings of an h1 element, this rule would apply to both 
    * Meaning - matches an element that is a sibling of antoher, although it does not have to be the directly preceding element. 

#### How CSS Rules Cascade 
- **Last Rule** If there are two or more rules that apply to the same element, it is important to understand which will take precedance. 
    * If two selectors are identical, the latter of the two will take precedence. 
- **Specificity** If one selector is more specific than the others, the more specific rule will take precedence over more general ones

#### Inheritance 
- If you specify the font-family of color properties on the `<body>` element they will apply to most child elements.  This is because the value of the front-family property is **inherited** by child elements. 
    * This saves you the time from having to apply these proprties to as many elemtns and results in a much simpler style sheet 
- You can force a lot of properties to inherit values from their parent elements by using inherit for the the value of the properties. 
