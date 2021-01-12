# Props and State

1. Does a deployed React application require a server?

  No, you can use html,css and js without node js[src](https://www.xspdf.com/resolution/55300177.html)

2. Why do we prefer to test a React application at the behavior rather than the unit level?

  Because we want to test for the user experiences rather than each of the possible units in order to deliver the required output.[src](https://testguild.com/unit-tdd-and-bdd-testing-whats-the-difference/)

3. What does npm run build do?

  It creates an optimized build of the app in the **build** folder.[src](https://reactjs.org/docs/create-a-new-react-app.html)

4. Describe the actual composition / architecture of a React application

  Multiple components and their own associated .scss files create a dynamic HTML structure that are imported into a main js file that renders and exports the collection of components to another file which retrieves the root element and renders the client view to ReactDOM.

  ## Terms

**BDD** - Behavior Driven Development

**Acceptance Tests** - Tests to ensure user needs, requirements and development process are satisfactory. [src](https://softwaretestingfundamentals.com/acceptance-testing/)

**mounting** - When React renders a component for the first time, building the initial document object model. [src](https://reacttraining.com/blog/mount-vs-render/#:~:text=%22Mounting%22%20is%20when%20React%20%22,initial%20DOM%20from%20those%20instructions.)

**build** - Command `npm run build` that creates an optimized build of the application in the **build** folder.

### PREP

[setState explained](https://css-tricks.com/understanding-react-setstate/)

[handling event](https://facebook.github.io/react/docs/handling-events.html)

[forms](https://facebook.github.io/react/docs/forms.html)

[state and lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)

[components and props](https://facebook.github.io/react/docs/components-and-props.html)

[React Testing Library](https://testing-library.com/docs/)

[RTL Testing Example](https://thomlom.dev/beginner-guide-testing-react-apps/)
