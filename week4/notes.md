# Week 4 Functions (part 2)

## agenda

- review quiz
- closures
- recursion

## closures

a closure is one function inside of(enclosed by) another.  
closures are useful because a closure gives you access to the outer function’s scope from the inner function.

    //a relatively common greeter example

    function greeting(greet) {
      return function(name){
        console.log(greet + ' ' + name);
      }
    }
    var sayHi = greeting('hello');
    sayHi('world');


>A closure is a special kind of object that combines two things: a function, and the environment in which that function was created. The environment consists of any local variables that were in-scope at the time that the closure was created.  
from [mdn](https://developer.mozilla.org/en/docs/Web/JavaScript/Closures)


## recursion

recursion is a common programming technique wherein a function calls itself inside of its own
function body

    function recur(){
      recur();
    }

this technique is often used because it can be easier to read than using loops..
