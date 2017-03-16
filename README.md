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

## Flex-alignment 

* Works on containers

```css

    /*justify-content: flex-start; default*/
    /*justify-content: flex-end;*/
    /*justify-content: center;*/
    /*justify-content: space-between;*/
    /*justify-content: space-around;*/
```
#### To align vertically

```css
    min-height: 100vh; /*Givin it height > contents is necessary else the container will end as soon as items are enclosed.*/
    flex-direction: column; /*change main axis from top to bottom*/
    justify-content: center; /*now the divs are aligned vertically in the center*/
```




