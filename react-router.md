# React Router

### Why use React Router

* Allows for a more robust way to render components
* It's very easy to use and configure

### How do we set it up

##### Step One

```
npm install -S react-router-dom
```

##### Step Two

Within Index.js

```
import { BrowserRouter as Router } from "react-router-dom";

// ...

ReactDOM.render(
  <Router>
    <App />
  </Router>,
  document.getElementById("root")
);
```

##### Step Three

```
import { Route, Link } from "react-router-dom";
```

##### Step Four

Within the navbar create links and in a seperate tage create a route

```
<Link to="">A Link</Link>
```

```
<main>
<Route path="" render= {} />
</main>
```

**Side Note** When using Link/Routes, the **to** and **path** need to be the same and in **Route** you need to render an actual component

### Additional Notes

**Redirect** is used to redirect the user back to a specific page if it does not exist or manually entered to the wrong page. It is usually placed at the end of the <Route />'s, needs to be imported with Link, Route

**Switch** this is placed around all of the <Route />'s and its key purpose is to have React Router go to and render the first matching result instead of checking all possible matching results.

**Sub Routes** are auxiliary views on the page, such as if we wanted to add a share component, without taking us or rendering a new page.

### Why is this so important

* Using Links/Routes/Switches/Redirects allows us to create quick links and pass information to our components.
* Allow us to ensure that users can't access incorrect web pages
* Allows us to redirect users if there are errors

### Additional Resources

[React-Router](https://git.generalassemb.ly/ga-wdi-lessons/react-router)
