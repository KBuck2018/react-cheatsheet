# Component Lifecycle Of The Rich & Famous

### Why is this important

Component Lifecycle is immensely important. One major reason is that it helps control the UI of a page so that certain aspects don't run until all the pieces have been created. This is vital when data is being accessed from a 3rd party API and needs to be displayed in a template.

### What makes the component lifecycle

The component lifecycle is made from two different methods, mounting and updating. Within each of these two methods are several lifecycle methods used throughout the application lifecycle.

### Whats within the mounting lifecycle

The mounting lifecycle has 5 methods

* constructor()
* componentWillMount()
* render()
* componentDidMount()
* componentWillUnmount()

Each of these methods are used during the various phases of the application.

### Whats within the updating lifecycle

The updating lifecycle has 5 methods

* componentWillReceiveProps()
* shouldComponentUpdate()
* componentWillUpdate()
* render()
* componentDidUpdate()

For more information on the methods within Updating and Mounting, please go to [here](https://reactjs.org/docs/react-component.html)

### Important Concepts

* **Uncontrolled Components** - sometimes it is better to let the DOM handle the data instead of ReactJS (which is a virtual DOM).

* **One Way Data Binding vs Two Way Data Binding** - **One way data binding** is where the user can input data but only the model has access to change the state of the app. **Two way data binding** is when the data changes so does the models data.

* When changing the state of the application in a function, you must bind the function in order for it to actually change state.

```
this.handleSubmit = this.handleSubmit.bind(this)
```

### Additional Resources

* [React Component Lifecycle](https://git.generalassemb.ly/ga-wdi-lessons/react-component-lifecycle)
* [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
