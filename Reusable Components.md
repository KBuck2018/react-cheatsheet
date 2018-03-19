# Reusable Components

### Why reusability is important

Reusability will allow you to make applications more efficient, thi can be done by making one function or method that can be used in multiple ways. Such as a form, if you have a website that has several different pages of forms, you can create a universal form once to cover however many forms you really need.

### Reasons why Reusable components are important:

* They allow for stronger building blocks in applications, if the reusable components work, then incorporating them in should work and allows for small progression quickly.

* Allow you to detect issues quicker, if an aspect of your reusable component breaks, the application is broken down into smaller components and will be easier to detect than something massive coding libraries.

### How are components broken down

#### Atoms Molecules Organisms

* **Atoms** are the smallest component or building block, they usually consist of one thing like text input, buttons, links, navbars, ect.

* **Molecules** consists of a couple atoms and generally make a functional compenent of an entire application, like putting a form together (several atoms) and adding a functional side, such as increasing or decreasing numbers, or adding names.

* **Organisms** are the complete product which includes all of the molecules and functionality.

To learn more about atoms/molecules/organisms please go [Here](http://bradfrost.com/blog/post/atomic-web-design/)

### Important To Remember

As you continue down developing ReactJs applications, you'll need to pass data or information from class to class. To ensure that the data that is being input or passed to components is correct, you'll need to use Proptypes.

#### What are PropTypes

PropTypes ensure that the data being sent to components is the right kind of data, such as a label atom asking for a name, does not send a number.

#### So wait how does that work?

* Well to start, you'll need to npm install prop-types

* Then you'll import prop-types on the .js file you want to add it to.

* Using prop-types, you can require specific bits of information such as the data being a string using syntax such as:

```
variableName.propTypes = {
    name: PropTypes.string.isRequired
}
```

* Another trick is that you can set the default values for the prop-types, this can be useful if you are using height and width for something, like an image or graph. This can be done by:

```
variableName.propTypes = {
    name: "Kevin"
}
```

### Why is this so important

It's important to realize how you can break applications down, from there you'll be able to not only tackle tough problems but make things mor efficient for not only you but anyone else adding components onto the application.

## Additional Resources

[Reusable Components](https://git.generalassemb.ly/ga-wdi-lessons/react-reusable-components)
