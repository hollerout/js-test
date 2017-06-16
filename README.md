# Javascript Technical Test
Welcome to our Javascript technical test! This test presumes you have knowledge of Javascipt and some ES6 syntax such as the arrow function syntax (eg. () => {}).

## Test Overview
We will be learning to do some functional programming using Javascript today! In its essence, functional programming is simply just using functions to build our application instead of using objects and classes. The main advantages we have using functional programming are greater code reuability, easier testing, and clearer/cleaner code leading to better maintainability and developer happiness.

To aid our functional programming in Javascript, we will be using the library [Ramda](http://www.ramdajs.com) that provides us with many built-in functions to be productive immediately. However, if you can't find the function you need in Ramda, feel free to write your own in this test.

## Evaluation Criteria
We will be evaluating your code based on how much fun you had and how easy it is to understand, maintain and extend your code. This includes (but not only limited) to good naming convention, consistent coding style, clean code, and DRY (Don't Repeat Yourself).

## Test Delivery
Please enter your test solution at http://ramdajs.com/repl/?v=0.23.0 and send us the URL.

Note that the URL actually contains your url-encoded solution.

## Background Reading
Please start reading the below 4 articles to understand what is Ramda and functional programming:
http://randycoulman.com/blog/2016/05/24/thinking-in-ramda-getting-started/
http://randycoulman.com/blog/2016/05/31/thinking-in-ramda-combining-functions/
http://randycoulman.com/blog/2016/06/07/thinking-in-ramda-partial-application/
http://randycoulman.com/blog/2016/06/14/thinking-in-ramda-declarative-programming/

You can refer to Ramda documentation here: http://ramdajs.com/docs/#
and also this useful cookbook: https://github.com/ramda/ramda/wiki/What-Function-Should-I-Use%3F

Now you can proceed to attempt the test below:

## Test

Given
```js
// There can be many other kinds of order status such as new, cancelled, etc
// Price is always an integer for simplicity
const orders = {
  kfc: {
    id: 'xbcysu',
    price: 23,
    status: 'closed'
  },
  macdonald: {
    id: 'Ujxmw2',
    price: 123,
    status: 'pending'
  },
  burgerKing: {
    id: 'Sh2kfy8',
    price: 56,
    status: 'pending'
  },
  pizzaHut: {
    id: '9xkMsn2',
    price: 99,
    status: 'closed'
  },
  lotteria: {
    id: 'jf8sh3',
    price: 38,
    status: 'new'
  }
}
```

1) Write a function using Ramda pipe that takes a single argument orders and return the total price of all orders.
2) Write a function using Ramda pipe that takes a single argument orders and return the total price of all pending orders.
3) Write a function using Ramda pipe that takes a single argument orders and return the total price of all closed orders.
4) Write a *curried* function that takes two arguments (status and orders) and return the total price in orders of the given status. eg. `totalPriceInOrdersByStatus('new')(orders) // => total price of all new orders``
5) Refactor your 2nd and 3rd functions with your 4th function.

Note: Please refactor your code before submission for the fairest evaluation.
