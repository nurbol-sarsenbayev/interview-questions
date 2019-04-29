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

#### 8. What should be a, so that expression `a == 1 && a == 2` returns `true`?
##### Answer:
```js
var a = {
  sum: 1, 
  valueOf: function() {
    return this.sum++;
  } 
}
```
