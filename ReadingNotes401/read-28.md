# Component Composition

1. Can a parent component access the state of a child component?

yes by using a callback function passed as a prop from the parent component.

2. What can be passed along in a prop variable?

a method for the child component to use in order to send back information by name the prop variable and passing it's state or other data. 

3. How can a child component “know” the state of another component?

Through information passed from a shared parent component or having child components of its own.

## TERMS

**component props** - Properties of a component

**component state** - The current values of props after sets occurring from handler functions/events that will change the values and change what is rendered.

**application state** - Where in an applications program the program is being executed and the memory stored for the app.[src](https://stackoverflow.com/questions/8102674/what-is-application-state#:~:text=An%20application%20state%20is%20simply,previous%20version%20of%20the%20page.)

### PREP

[react basics](https://medium.freecodecamp.org/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030)

[props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

[composition vs inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)

[react testing library api ex](https://testing-library.com/docs/react-testing-library/example-intro)