#### 1. Write overload constructors to class Person, so that you can create instance of the class like `new Person()`, `new Person({ name: 'Nurbol', age: 27, isMale: true })`, `new Person({ name: 'Nurbol', age: 27 })` and `new Person('Aigerim', 25, false)`
```ts
class Person {
  name: string = 'Unknown';
  age: number = 0;
  isMale: boolean = true;
}
```
##### Answer:
```ts
class Person {
    name: string = 'Unknown';
    age: number = 0;
    isMale: boolean = true;

    constructor();
    constructor(init: Partial<Person>);
    constructor(name: string, age: number, isMale: boolean);  
    constructor(initOrName?: Partial<Person> | string, age?: number, isMale?: boolean) {
      if (initOrName) {
        if (typeof initOrName === 'object') {
            Object.assign(this, initOrName);
        } else {
            Object.assign(this, { name: initOrName, age, isMale });
        }
      }
    }
}
```
