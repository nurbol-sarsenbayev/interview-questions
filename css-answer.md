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
