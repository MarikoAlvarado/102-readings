# Routing

1. Do child components have direct access to props/state from the parent?

No, but they can be given prop methods to send back data to the parent in order to set states.

2. When a component “wraps” another component, how does the child component’s output get rendered?

The child component can be rendered once the conditions of the parent components have been met and the child component will adhere to the structure set by the parent.

3. Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?

Yes

4. What trick can a parent use to share all props with it’s children

`DisplayAllProps` with the spread operator.[src](https://medium.com/coding-at-dawn/how-to-pass-all-props-to-a-child-component-in-react-bded9e38bb62)

# Terms

**props.children** - used to display whatever is included between open and closing tags when invoking a component.[src](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

**composition** - A way of reusing code between components.[src](https://reactjs.org/docs/composition-vs-inheritance.html)

#### prep

[browser router tutorial](https://blog.pshrmn.com/entry/simple-react-router-v4-tutorial/)

[browser router api docs](https://reacttraining.com/react-router/web/api)