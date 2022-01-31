1. Using loops take 10 inputs from user and find the average of all the numbers.

let count = 1;
let add_1 = 0;
while(count <= 10){
    let num = +prompt(`Enter the number : `);
    add_1 += num;
    
    num = 0;
    count ++;

}
let average = add_1 / 10;
console.log(average);

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```

println is not defined.



3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

function getEvenSum(max){
    let count = 0;
    let even = 0;
        while(count <= max){
            if(count % 2 == 0){
                even += count;
            }
            count ++;
        }
    console.log(even);
    }
getEvenSum(10);


4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

function getOddSum(max){
    let count = 0;
    let odd = 0;
        while(count <= max){
            if(count % 2 != 0){
                odd += count;
            }
            count ++;
        }
    console.log(odd);
    }
getOddSum(10);

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

function getProductOfDigits(n)
{
    let product = 1;
     if(n > 0){
        while (n != 0){
        product = product * (n % 10);
        n = Math.floor(n / 10);
        }
        return product;
      } else {
        return `Enter the number greater then 0`;
     }
}
 getProductOfDigits(123); 

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.


6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); number is greater then 5 because the argument we are calling is greater then 5
check(1); number is smaller then 5 because the argument we are calling is less then 5
check(5); 5 because there is no condition for the number if it is equal to 5

```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); "You are arya" because in the condition we are returning You are arya
getOutput('John'); "You are john" because in the condition we are returning You are john

getOutput(); Who are you because in the condition we are returning Who are you
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // what will be the output
getOutput('John'); // what will be the output
getOutput(); // what will be the output
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

no

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
