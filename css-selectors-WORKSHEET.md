
# CSS Worksheet
To preview a markdown file in VS Code:

Ctrl + SHIFT + V


## Problem 1
Explain the difference between these two selectors (make sure to mention the elements that each selector is targeting):
```css
ul li.selected{
	/*rules (property settings) go here*/
}


ul li .selected{
	/*rules (property settings) go here*/
}
```
### Put your answer here

The difference between them is the space between li and the class selected. The li.selected is selecting the li.selected while li .selected is selecting elements nested inside the li.

## Problem 2
What are **square brackets** used for in CSS selectors?
For example, what does the following selector target:
```css
input[type=text]{
	/*rules (property settings) go here*/
}
```
### Put your answer here

Square brackets are used for attributes. It allows it so you can target certain elements based on their attributes.

## Problem 3
What is the **greater than** character used for in CSS selectors?
For example, what does the following selector target:
```css
div > p{
	/*rules (property settings) go here*/
}
```
### Put your answer here

The greater than characters is called the child combinator. It's used to select elements that are the direct children of another element. So for the example it would be selecting p elements that are the immediate children of the div element.

## Problem 4
What is the **tilde** used for in CSS selectors?
For example, what does the following selector target?
```css
h3 ~ p{
	/*rules (property settings) go here*/
}
```
### Put your answer here

The tilde is a sibling selector. It selects all elements that share the same parent and comes after a specified element. In the example it's selecting any p elements after the h3 element.

## Problem 5
What is the **+** sign used for in CSS selectors?
For example, what does the following selector target:
```css
input[type=radio] + label{
	/*rules (property settings) go here*/
}
```
### Put your answer here
The plus selector targets an element that immediately follows another specific element and also shares the same parent. In the example it means that its selecting the label element that comes after the radio input. 


## Problem 6
Explain what a **psuedo selector** is in CSS.
And include a code sample that demonstrates a psuedo selector.
### Put your answer here
A pseudo selector lets CSS style an element when something special is happening to it.  

p:hover {
	color: blue;
}
<p>Hover over this text </p>
So what happens is that once you hover over the p element, it'll turn blue.