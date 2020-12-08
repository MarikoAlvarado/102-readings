# Node Ecosystem, TDD, CI/CD

**1. What does `array.map()` do?**

`Array.map()` calls a function for each element in an array and returns a new array.

**2. What does `array.reduce()` do?**

`Array.reduce()` takes an accumulator and a value. The value of each array element is tested against a function. whatever value the function returns is stored in the accumulator and by the end of the process, the array has been reduced down to a single value which can be returned as a string, array or an object.

**3.Code snippets for how to us `superagent()` to fetch data from a URL and log result**

**Normal Promise using `.then()`**

```
superagent.get(urlHere)
.then(dataFromUrl=>{
  console.log(dataFromUrl.body)
})
```

**Using `async/await`**

```
async function getData(){
    let urlData = await superagent.get(urlHere)
    console.log(urlData.body)
  }
  getData();
```

**4. What are promises?**

A promise can be stated explicitly or implicitly. The code which the promise depends on can either **resolve** or **reject** the promise.

**5. Are callback functions considered to be Asynchronous**

Not all callback function are asynchronous because some callbacks can be called as regular functions while an async function is a reference/argument from another function that will run and when finished will allow the function it was passed through to complete. [source](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Introducing#:~:text=Async%20callbacks%20are%20functions%20that,something%20of%20interest%20has%20happened.)

