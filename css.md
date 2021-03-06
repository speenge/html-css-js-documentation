# CSS documentation:

## Syntax:
    selector {declaration; declaration;}
    h1 {color:#1e1e3f; font-size:16px;}

    Typical syntax:
        p {
            color: red;
            text-align: center;
        }


## Selector:
    p {
        color: blue;
    }
 ^Here all the `<p>` elements would have the text color blue.
___________________________________

    #id_1 {
        color: green;
    }
^Here all elemnts tagged with the `id="id_1"` will have the text color green.
___________________________________

```
    .center {
        text-align: center;
    }
```
^All elements tagged with `class="center"` wil be center aligned.
___________________________________

```
p.center {
    color: yellow;
    text-align: center;
}
```
^Only `<p>` elements with `class="center"` will get the above style.
___________________________________

    <p class="center large">This paragraph refers to two classes.</p>
    (I believe that is decided by the space in the class string.)
___________________________________

```
* {
    color: blue;
}
```
### ^The wildcard character strikes again(affects every HTML element on the page)
___________________________________
    
    You can group selectors with commas
    
```
h1, h2, p {
    text-aligned: center;
    color: red;
}
```
### ^gives the tags `<h1> <h2>` and `<p>` center aligned text and the color red.


## All CSS Simple Selectors:
```
Selector	        Example	Example description
#id	                #firstname      Selects the element with id="firstname"
.class              .intro          Selects all elements with class="intro"
element.class       p.intro	        Selects only <p> elements withclass="intro"
*                   *               Selects all elements
element             p               Selects all <p> elements
element,element,..	div, p	        Selects all <div> elements and all <p>elements
```


## Add CSS:
- External CSS
- Internal CSS
- Inline CSS

### External CSS:
Put this in the `<head>` tag to define the css file:
    `<link rel="stylesheet" href="style.css">`
    
### Internal CSS:
Is defined in the `<style>` element, which most often is in the `<head>` element

### Inline CSS:
Is defined with the style attribute of the relevant element
`<h1 style="color:red;">header1</h1>`
The Inline style loses many of the advantages of a stylesheet
        
## CSS grid:
- grid-column-start
- grid-column-end
- grid-column
- grid-row
- order
- grid-template-columns
- grid-template-rows
- grid-template


### grid-column-start:
Starts the grid column at the set value.

### grid-columnn-end:
Stops the grid column at the next value 5 equals column 4 visually.

### grid-column:
Sets the start and end of the column:
        `grid-column: 1 / 5;`
        starts the grid at 1 & ends it visually at 4.

### grid-row:
Works the same as grid-column but it's for the rows instead.

### order:
 manipulates the order something is shown can take positive & negative numbers.

### grid-template-columns:
Sets the size of the columns in the grid, can be in px, em precentages and you can even mix different units together.

### grid-template-rows:
Works the same as grid-template-columns just for the rows.

### grid-template:
Is a shorthand for the grid-template-columns and grid-template-rows.
``` 
grid-template: 20% 20% 20% 20% 20% / 50% 50%;
```
^Sets the grid to have 5 rows that each is 20% and tow columns that are 50% of the allowed space for the div.

[temp test link](https://github.com/gigalomaniacx/html-css-js-documentation/blob/main/linkTest.md)