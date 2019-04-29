#### 1. How many ways do you know positioning block in parent horizontally and vertically?
```html
<div class="parent">
  <div class="child"></div>
</div>
```
##### Answer1:
```css
  .parent {
    display: flex;
    justify-content: center;
    align-items: center;
  }
```
##### Answer2:
```css
  .parent {
    position: relative;
  }
  .child {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
```
#### 2. Say size of margin top and margin left of child block in pixels?
```html
<div class="parent">
  <div class="child"></div>
</div>
```
```css
.parent {
  width: 400px;
  height: 300px;
}

.child {
  width: 100px;
  height: 50px;
  margin-top: 50%;
  margin-left: 50%;
}
```
##### Answer:
The size of the margin as a percentage, relative to the width of the containing block.
```css
margin-top: 200px;
margin-left: 200px;
```
#### 3. Given a button. When pressed, the button should rise by one pixel without affecting the remaing elements. Implement it using only css.
```html
<button class="btn">Button</button>
```
##### Answer:
```css
.btn:active {
  position: relative;
  top: -1px;
}
```
#### 4. What will be actually size of element in pixel?
```css
.block {
  width: 300px;
  height: 100px;
  border: 1px solid blue;
  padding: 10px;
  margin: 10px;
}
```
##### Answer:
width + padding + border = actual width of an element so width = 322px
height + padding + border = actual height of an element so height = 122px
#### 5. What css property should be added so that the actual width of the element is 300px and the height is 100px?
##### Answer:
```css
.block {
  width: 300px;
  height: 100px;
  border: 1px solid blue;
  padding: 10px;
  margin: 10px;
  box-sizing: border-box;
}
```
#### 6. What do you know about css positions?
#### 7. What do you know about display: flex?
#### 8. What do you know margin collapse?
#### 9. What do you know about css display property?
#### 10. What is difference between display: inline and display: inline-block?
##### Answer:
For inline elements don't effect these css properties: width, height, margin-top, margin-bottom, padding-top, padding-bottom
#### 11. What do you know about padding, margin and border?
#### 12. What pseudo classes and pseudo elements do you know in css?
##### Answer:
::after, ::before, :focus, : blur, :active, :hover
#### 13. What do you know about `::after` and `::before` pseudo elements?
#### 14. Tell about pseudo class `:last-child` and `:first-child`. What color will in each paragraphs?
```html
<section>
  <p>Один</p>
  <div>Uno</div>
  <p>Два</p>
  <div>Dos</div>
  <p>Три</p>
  <div>Tres</div>
</section>
```
```css
p {
  color: red;
}
p:first-child, p:last-child {
  color: blue;
}
```
##### Answer:
The first paragraph will be red. The other will be blue. Because, initially, the last element is selected, then it is checked that it is `<p>` element.
[Link to material](https://webref.ru/layout/structural-pseudo-classes/first-child)

#### 15. 

#### 13. Write css selector for elements with attribute `data-target`. For elements which data-target attribute has value `call-modal`.
##### Answer:
```css
[data-target] { }
[data-target="call-modal"] { }
```
#### 14. What do you know about adaptive design? How implement it in css?
#### 15. About media query, break points?
#### 18. Tell about BEM methodology.
##### Answer:
BEM - Block, Element and Modicificator
