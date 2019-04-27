#### 1. How many ways do you know positioning block in parent?
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
