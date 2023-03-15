<ol>
<li>

**What will be the output?**

```JS
const fruits_obj = { 0 : "apple" , 1 : "mango" ,  2:"banana"};
const fruits_arr = ["apple","mango", "banana"];

console.log(typeof fruits_obj);
console.log(typeof fruits_arr);
console.log(fruits_obj == fruits_arr);
```

- A: `Object , Array , False`
- B: `Object , Array , True`
- C: `Object , Object , False`
- D: `Object , Object , True`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>
</li>

<li>

**What will be the output ?**

```JS
if (true) {
  function foo() {
    console.log(1);
  }
} else {
  function foo() {
    console.log(2);
  }
}

foo();
```

- A: `1`
- B: `2`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>

</li>

<li>

**What will be the output ?**

```JS
for (var i = 0; i < 4; i++) {
  setTimeout(() => console.log(i), 0)
}

```

- A: `0 1 2 3`
- B: `4 4 4 4`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>
</li>

<li>

**What is the output ?**

```JS
const animal = {
  animal_name: "cat",
  action: function () {
    console.log(`${this.animal_name} is doing action`);
  }
};

setTimeout(animal.action, 1000);

```

- A: `cat is doing action`
- B: `undefined is doing action`
- C: `null is doing action`
- D: `error`

<br/>

<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>

</li>

<li>

**Guess the following output?**

```JS
let array = [1, 2, 3];
let array2 = array;
let array3 = [...array];

console.log(array.concat(4));
console.log(array2.concat(5));
console.log(array3.concat(6, 7));
```

- A: `[ 1, 2, 3, 4 ], [ 1, 2, 3, 5 ], [ 1, 2, 3, 6, 7 ]`
- B: `[ 1, 2, 3, 4, 5 ], [ 1, 2, 3, 4, 5 ], [ 1, 2, 3, 6, 7 ]`
- C: `[ 1, 2, 3 ], [ 1, 2, 3, 4, 5 ], [ 1, 2, 3, 6, 7 ]`
- D: `[ 1, 2, 3, 4 ], [ 1, 2, 3, 5 ], [ 1, 2, 3, 6, 7 ]`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>
</li>

<li>

**What will be the output?**

```JS
let array = [1, 2, 3, 4, 5, 6];
let [a, b, , ...rest] = array;

console.log(a)
console.log(b)
console.log(c)
console.log(rest)
let c;
```

- A: `1, 2, 3, [ 4, 5, 6 ]`
- B: `1, 2, c is not defined`
- C: `1, 2, NaN, undefined`
- D: `1, 2, c is not defined, [4, 5, 6]`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>
</li>

<li>

**Guess the following output?**

```JS
const nums = [1, 2, 3, 4, 5, 6];

const res = nums.forEach((item) => {
  return item * item;
});

console.log(res);
```

- A: `null`
- B: `[ 1, 4, 9, 16, 25, 36 ]`
- C: `[1, 2, 3, 4, 5, 6]`
- D: `Undefined`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: D

</p>
</details>
</li>

<li>

**What will be the output?**

```JS
const example = ({ a, b, c }) => {
 console.log(a, b, c);
};
example(0, 1, 2);
```

- A: `undefined, undefined, undefined`
- B: `0 undefined undefined`
- C: `0, 1, 2`
- D: `None of the above`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>
</li>

<li>

**When do we say that a promise is 'settled'?**

- A: `If it is fulfilled`
- B: `If it is rejected`
- C: `If it is pending`
- D: `If it is either fulfilled or rejected`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: D

</p>
</details>
</li>

<li>

**Which of the following isn’t a method of Javascript Promise?**

- A: `Promise.then()`
- B: `Promise.all()`
- C: `Promise.error()`
- D: `Promise.catch()`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
class Chameleon {
  static colorChange(newColor) {
    this.newColor = newColor;
    return this.newColor;
  }

  constructor({ newColor = 'green' } = {}) {
    this.newColor = newColor;
  }
}

const freddie = new Chameleon({ newColor: 'purple' });
console.log(freddie.colorChange('orange'));
```

- A: `orange`
- B: `purple`
- C: `green`
- D: `TypeError`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: D

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
let greeting;
greetign = {}; // Typo!
console.log(greetign);
```

- A: `{}`
- B: `ReferenceError: greetign is not defined`
- C: `undefined`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
function Person(firstName, lastName) {
  this.firstName = firstName;
  this.lastName = lastName;
}

const member = new Person('Lydia', 'Hallie');
Person.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};

console.log(member.getFullName());
```

- A: `TypeError`
- B: `SyntaxError`
- C: `Lydia Hallie`
- D: `undefined` `undefined`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
function checkAge(data) {
  if (data === { age: 18 }) {
    console.log('You are an adult!');
  } else if (data == { age: 18 }) {
    console.log('You are still an adult.');
  } else {
    console.log(`Hmm.. You don't have an age I guess`);
  }
}

checkAge({ age: 18 });
```

- A: `You are an adult!`
- B: `You are still an adult.`
- C: `Hmm.. You don't have an age I guess`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>
</li>

<br />
<li>

**How long is MY_SECRET accessible?**

```JS
sessionStorage.setItem('MY_SECRET', 123);
```

- A: Forever, the data doesn't get lost.
- B: When the user closes the tab.
- C: When the user closes the entire browser, not only the tab.
- D: When the user shuts off their computer.

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
const obj = { a: 'one', b: 'two', a: 'three' };
console.log(obj);
```

- A: `{ a: "one", b: "two" }`
- B: `{ b: "two", a: "three" }`
- C: `{ a: "three", b: "two" }`
- D: `SyntaxError`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
function sayHi() {
  return (() => 0)();
}

console.log(typeof sayHi());
```

- A: `"object"`
- B: `"number"`
- C: `"function"`
- D: `"undefined"`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: B

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
// counter.js
let counter = 10;
export default counter;
```

```javascript
// index.js
import myCounter from "./counter";

myCounter += 1;

console.log(myCounter);
```

- A: `10`
- B: `11`
- C: `Error`
- D: `NaN`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: C

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
const name = 'Lydia';
age = 21;

console.log(delete name);
console.log(delete age);
```

- A: `false`, `true`
- B: `"Lydia"`, `21`
- C: `true`, `true`
- D: `undefined`, `undefined`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>
</li>

<br />
<li>

**What's the output?**

```JS
const settings = {
  username: 'Holaa',
  level: 19,
  health: 90,
};

const data = JSON.stringify(settings, ['level', 'health']);
console.log(data);
```

- A: `"{"level":19, "health":90}"`
- B: `"{"username": "Holaa"}"`
- C: `"["level", "health"]"`
- D: `"{"username": "Holaa", "level":19, "health":90}"`

<br/>
<details>
<summary><b>Answer</b></summary>
<p>

#### Option: A

</p>
</details>
</li>

</ol>
