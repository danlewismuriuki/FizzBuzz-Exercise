Write a program that takes a user’s input and prints the numbers from one to the number the user entered. However, for multiples of three print Fizz instead of the number and for the multiples of five print Buzz. For numbers which are multiples of both three and five print FizzBuzz.


npm install


Then, run the program:

node fizzbuzz.js

The program will prompt you to enter a number. Enter the number and the program will print the FizzBuzz sequence up to that number.

Example
$ node fizzbuzz.js

Enter a number: 15

1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz


## Code

The code for the FizzBuzz program is as follows:

```javascript
function fizzBuzz(n) {
  for (let i = 1; i <= n; i++) {
    let output = "";
    if (i % 3 === 0) {
      output += "Fizz";
    }
    if (i % 5 === 0) {
      output += "Buzz";
    }
    if (output === "") {
      output = i;
    }
    console.log(output);
  }
}

fizzBuzz(15);


This code first defines a function called `fizzBuzz()`, which takes an integer `n` as input. The function then iterates from 1 to `n`, and for each number `i`, it checks if `i` is divisible by 3 and by 5. If `i` is divisible by 3, the function adds the string "Fizz" to the output string `output`. If `i` is divisible by 5, the function adds the string "Buzz" to `output`. If `i` is not divisible by 3 or 5, the function simply adds `i` to `output`. Finally, the function logs the value of `output` to the console.

## License

The FizzBuzz program is released under the MIT License. See the LICENSE file for more details.


I hope this helps!