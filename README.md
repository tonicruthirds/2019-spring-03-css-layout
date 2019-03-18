# CoderBabez

##  Week Three - CSS Layouts

### Objectives
Use flexbox to create a complex site layout with rows and columns.

### Vocab
* Box Model
* Divs
* Parent Elements
* Child Elements
* Flexbox

### Review
1. What tags are used on this page?
2. What styles are used on this page?
3. How does the html page know about the styles?

![alt text](https://github.com/megknoll/coderbabez-css-wk2/raw/master/img/practice.png "Review")

### Intro
Last week we started exploring using CSS to add styles to our pages. This week we're going to continue with CSS to work on layout - or moving elements to specific positions on the page using CSS.

### Lesson - CSS and Layouts:

1. When you look at HTML, imagine every element having a box drawn around it. In CSS, the term "box model" is used when talking about design and layout. The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content.

![alt text](https://github.com/megknoll/coderbabez-css-wk2/raw/master/img/boxmodel.png "Box Model")

2. Sometimes we want to group these boxes together into larger boxes that can be styled as a single section. When we want to do that, we can use the `<div>` tag. Think of the div tag a blank slate / empty box.

3. When we nest tags inside of each other (like with a div), we call the outer element the parent and the inner element the child.

![alt text](https://github.com/megknoll/coderbabez-css-wk2/raw/master/img/child_parent_element.png "Parent vs. Child Element")

4. The ability to group items together like this becomes especially useful when we want to create complex layouts like rows and columns. There are a few ways to do this in CSS. The most common way to create layouts is something called a "float", but today we're going to use a new CSS method called "flexbox". Flexbox is more modern, and is probably what most sites will use in the future, even though some older browsers don't support it.

5. In flexbox, the parent element tells the child elements how to behave.
```html
<div class=”parent”>
	<div class=”child”>
		<img ...>
	</div>
</div>
```

This CSS is telling all of the elements inside of the parent tag to appear in a centered column.
```css
parent {
	display: flex;
	flex-direction: column;
	align-items: center;
}

```

Look at the flexbox cheat sheet below for more flexbox rules you can use!

### FlexBox Cheat Sheet

display: sets the flex container
* flex

flex-direction: sets the main axis for the content
* row
* row-reverse
* column
* column-reverse

justify-content: defines how items are aligned along the main axis.
* flex-start
* flex-end
* space-around
* space-between
* center

align-items: defines how items are aligned along the secondary or cross axis.
* flex-start
* flex-end
* center
* stretch

flex-wrap: tells us if the content should wrap, or try to fit on one line
* nowrap
* wrap
* wrap-reverse

### Practice Together
1. Open up the index.html file in the practice folder of this repo
2. Use flexbox to make the boxes centered in a column on the page
3. Use flexbox to make the boxes in a column on the right side of the page
4. Use flexbox to reverse the order of the boxes in a row in the vertical center of the page. All of the items should have even space around them.

### Practice on Your Own:
Go to the superhero supply shop repo and follow the homework instructions!

### Final Thoughts
Today we learned how we can use CSS to add style and layouts to our pages.
Next week we’ll do our first big review project and make our own portfolio pages.
