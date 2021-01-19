# Hooks API

1. Why do we not need more .html pages in a multi-page React app?

Because one html page can serve as the template where all of the components will be rendered to by ReactDOM to the root div within the html body.

2. If we wanted a component to show up on every page, where would we put it and why?

Inside the <BrowserRouter />, outside a <Route /> - I'm not sure why exactly. I would guess it's because the components should be recognized as a route within BrowserRouter but outside of the routes themselves as a overall applicable components whenever the specific routes are rendered.


3. What does props.children contain?
It's a property that can be passes to any component if referred to as props.children to render information. [src](https://codeburst.io/a-complete-guide-to-props-children-in-react-c315fab74e7c)

# Terms

**Composition** - A natural pattern of the component mode used to build components using other component through the use of props.[src](https://dev.to/bouhm/thinking-in-react-component-composition-fp5)

**Children / Child Components** - Dependent on parent components for information through props sent from parents in order to render content/send back information.

**Hash Routing** - uses the hash portion of URL to keep UI in sync with URL[src](https://reactrouter.com/web/api/HashRouter)

**Link Routing** - Declarative, accessible navigation around the application[src](https://reactrouter.com/web/api/HashRouter)



#### prep

[making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

[the state hook](https://reactjs.org/docs/hooks-state.html)

[hooks api](https://reactjs.org/docs/hooks-overview.html)

[hooks api reference](https://reactjs.org/docs/hooks-reference.html)

[effects hook](https://reactjs.org/docs/hooks-effect.html)