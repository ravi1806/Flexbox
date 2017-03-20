# Flexbox by [Wes Bos](https://flexbox.io/) 

## Flex-direction 

* Works on containers. 

```css
   flex-direction : row; /* Default, wherein the main axis goes from left to right, cross axis from top to bottom. */
   flex-direction : column; /* Main axis goes from top to bottom. */
   flex-direction : row-reverse; 
   flex-direction : column-reverse;
```

## Flex-wrap

* Works on containers.

```css
   flex-wrap: wrap; 
```

## Flex-ordering

* Works on flex items
  1. Default order on flex items is 0.
  1. A higher order takes the item to right.
  1. A lower order takes the item to left.
  1. Negative values of order are legit.

```css
   order: SOMENUMERICALVALUE;
```

## Flex-alignment with justiy-content

* Works on containers

```css

    justify-content: flex-start; /*default*/
    justify-content: flex-end;
    justify-content: center;
    justify-content: space-between;
    justify-content: space-around;
```
#### To align vertically

```css
    min-height: 100vh; /*Givin it height > contents is necessary else the container will end as soon as items are enclosed.*/
    flex-direction: column; /*change main axis from top to bottom*/
    justify-content: center; /*now the divs are aligned vertically in the center*/
```

## Flex-alignment with align-items

* Works on containers
* Works on cross axis(!important point to notice) cos align-items:center wont work on main axis.

```css
     align-items: stretch; /*default*/
     align-items: center; /*this aligns the item across the cross axis, not the main axis, so give container some height*/
     height: 100vh; /*Without height it wont be able to center across the cross axis.*/
     align-items: flex-end;
     align-items: baseline; /*will align to the base of the text in each box*/
```
## Flex-alignment with align-contents

* Works on containers
* Works only on cross axis
* Removes previously defined heights on boxes 
* needs wrap

```css
    flex-wrap: wrap; /*align content requires wrap around to work*/
    align-content: stretch; /*default*/
    align-content: flex-start;
    align-content: flex-end;
    align-content: space-between;
    align-content: space-around;
    align-content: center;
```
## Flex-alignment with align-self

* Works on flex items.
* Wors on cross axis
* Removes previously defind heights on items

```css 
   .box1 {
     align-self: stretch;
     align-self: flex-start;
     align-self: center;
     align-self: flex-end;
    }
```


