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
#### 2. How many pixels margin top and margin left of child block?
```html
<div class="parent">
  <div class="child"></div>
</div>
```
```css
.parent {
  width: 400px;
  height: 300px;
  border: 1px solid red;
}

.child {
  width: 100px;
  height: 50px;
  background: red;
  margin-top: 50%;
  margin-left: 50%;
}
```
##### Answer:
percentage is calculated to relative to the parent container's width
```css
margin-top: 200px;
margin-left: 200px;
```
