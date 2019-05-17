#### 1. You have function calc. Below given executions of this function. Say the results of these executions and their types 
```javascript
function calc(n = 5) {
	return n + 5;
}
```
1. `calc()`
2. `calc(null)`
3. `calc("")`
4. `calc(undefined)`

#### 2. How this code will work? Explain it.
```javascript
let letter = 'A';
switch(letter) {
	case 'A':
		const x = 2;
		console.log('A', x);
	case 'B':
		console.log('B', x);
}
console.log('Last', x);
```
#### 3. How this code will work?
```javascript
let letter = 'B';
switch(letter) {
	case 'A':
		const x = 2;
		console.log('A', x);
	case 'B':
		console.log('B', x);
}
```
#### 4. What will see in console? Why?
```js
class Base {
	constructor() {
		this.name = 'Base';
		this.getName = () => {
			return this.name;
		}
	}

	say(str) {
		console.log(`${this.getName()}: ${str}`);
	}
}

class Child extends Base {
	constructor() {
		super();
		this.name = 'Child';
	}

 	getName() {
		return 'Child2';
	}
}

const c = new Child();
console.log(c.name);
console.log(c.getName());
console.log(c.say('Hello'));
```
#### 5. What do know about events focus and blur?

#### 6. What attribute you should add div element, so that it can trigger focus and blur events?

#### 7. What is `instanceof` used for? How it works?

#### 8. What should be `a`, so that expression `a == 1 && a == 2` returns `true`?
##### Answer:
```js
var a = {
  sum: 1, 
  valueOf: function() {
    return this.sum++;
  } 
}
```
#### 9. How to clone object except one defined property using ES6?
##### Answer:
```js
const { x, ...rest } = obj;
const clonedObj = { ...rest };
```
#### 10. What will be the value of the text element, when we click on the button?
```html
<input type="button" id="button" value="Нажми меня">
<input type="text" id="text" size="60">

<script>

  button.onclick = function() {
    text.value += ' ->в onclick ';

    text.focus();

    text.value += ' из onclick-> ';
  };

  text.onfocus = function() {
    text.value += ' !focus! ';
  };
</script>
```
##### Answer:
The value of the text element will be " ->в onclick  !focus!  из onclick-> " 
#### 11. When events are processed synchronously?
##### Answer:
When an event is triggered not by a visitor, but by code. Example:
```js
elem.focus();
```
#### 12. What is the main difference between yarn and npm?
##### Answer:
Using yarn, you can add cashed packages when you are offline.
#### 13. What do you know about DOM and BOM?
