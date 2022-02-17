# Conditional Statements

If we want to write commands that handle different decisions in your code then we can use conditional statements based on different conditions. 

## if Statement

Use **if** to specify a block of code to be executed, if a specified condition is true.

### Syntax:
```
if (pet === 'dog'){
    console.log("I own a dog");
} 
```

## else Statement

Use **else** to specify a block of code to be executed, if the same condition is false.

### Syntax:
```
if (pet === 'dog'){
    console.log("I own a dog");
} else {
    console.log("I don't own a pet")
}
```

## else if Statement

Use **else if** to specify a new condition to test, if the first condition is false.

### Syntax:
```
if (pet === 'dog'){
    console.log(`I own ${pet}`);
} else if(pet === 'cat') {
    console.log(`I own ${pet}`);
} else {
    console.log("I don't own a pet");
}
```

## switch Statement

Use **switch** to specify many alternative blocks of code to be executed.
switch statements can have a cleaner syntax over complicated if else statements.

### Syntax:
```
switch (pet) {
    case 'dog':
        console.log('I own a dog');
        break;
    case 'cat':
        console.log('I own a cat');
        break;
    case 'parrot':
        console.log('I own a parrot');
        break;
    default:
        console.log('I dont own a pet');
        break;
}
```

# Loops

Loops are used in JavaScript to perform repeated tasks based on a condition. Conditions typically return true or false when analysed. A loop will continue running until the defined condition returns false

## for loop

**for** - loops through a block of code a number of times.

### Syntax
```
for (statement 1; statement 2; statement 3) {
  // code block to be executed.
}

for (let i = 0; i < 9; i++) {
  console.log(i);
}

for (let i = 1; i <= arr.length; i++) {
    console.log(arr[i]);
}
```

**Statement 1**: It is also called as initialization. Run before the first execution on the loop. This expression is commonly used to create counters. Variables created here are scoped to the loop. Once the loop has finished its execution they are destroyed.

**Statement 2**: Here we write the condition. This expression/condition checked before the execution of every iteration. If it evaluates to true, the loop’s statement is executed. If it evaluates to false, the loop stops.

**Statement 3**: The expression that is run after every iteration. This is usually used to increment a counter, but can be used to decrement a counter instead.

## for in loop

**for/in** - The for...in statement iterates over the properties of an object.

### Syntax
```
for (let key in obj){
    console.log(key + ':' + obj[key]);
}
```

## for of loop

**for/of** - statement iterates of the values of many types of iterables, including arrays, and special collection types like Set and Map.

### Syntax
```
for (variable of iterable) {
  // code block to be executed.
}
```

## while loop

**while** -The while loop starts by evaluating the condition. If the condition is true, the statement(s) is/are executed. If the condition is false, the statement(s) is/are not executed. After that, while loop ends.

### Syntax
```
while (condition) {
  // code block to be executed.
}

while (i <= 10) {
    console.log(i);
    i++;
}
```

## do while loop

**do/while** - The do...while loop is closely related to while loop
Do...While loops makes sure that the code is executed at least once, and after the execution, if the condition inside the while() is true, it continues with the loop, otherwise it stop.

### Syntax
```
do {
  // code block to be executed.
}
while (condition);

let i = 10;

let ar = [];

do {
    ar.push(i);
    i++;
} while(i<=10);

console.log(ar);
```
