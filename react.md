# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:
All are true

- React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs)
- React is a modern, efficient answer to complex UI applications
- React is a full stack framework for modern web applications
- React is a flexible library that plays the role of V in an MVC framework
//MVC - Model View Controller


 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.


 //Your Answer
Dumb components do not have state.  Smart components have state.  Components with state create the initial display of the UI. Functions can be applied to state to update the data.  Or, state can be passed down via props to the child component.

 //Googled Answer
Smart and dumb components is a concept I learnt from React. Smart components are also called containers, they are the ones who handle the state changes, they are responsible for how things work. On the opposite, the dumb components, also called presentational, only handle the look and feel.

#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?


 //Your Answer
 yarn is updating all files in the specified directory


 //Googled Answer
 In general, a package is simply a folder with code and a package.json filethat describes the contents. When you want to use another package, you firstneed to add it to your dependencies. This means running yarn add [package-name]to install it into your project.This will also update your package.json and your yarn.lock so that otherdevelopers working on the project will get the same dependencies as you whenthey run yarn or yarn install


#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

    import React, { Component } from 'react';

    class Recipes extend Component {
      constructor(props){
        super(props)
        this.state = {
          recipes:
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}

        }
      }

      render() {
        let { recipes } = this.state
        return (

          let recipes = this.state.recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li> ???
            )
          })

          <ul>
            {recipes}
          </ul>
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)

 //Your Answer
button, checkbox, color

 //Googled Answer
The HTML <input> element is used to create interactive controls for web-based forms in order to accept data from the user; a wide variety of types of input data and control widgets are available, depending on the device and user agent.  How an <input> works varies considerably depending on the value of its type attribute, hence the different types are covered in their own separate reference pages. If this attribute is not specified, the default type adopted is text.
The available types are as follows:
button: A push button with no default behavior.
checkbox: A check box allowing single values to be selected/deselected.
color: HTML5 A control for specifying a color. A color picker's UI has no required features other than accepting simple colors as text (more info).
date: HTML5 A control for entering a date (year, month, and day, with no time).
datetime-local: HTML5 A control for entering a date and time, with no time zone.
email: HTML5 A field for editing an e-mail address.
file: A control that lets the user select a file. Use the accept attribute to define the types of files that the control can select.
hidden: A control that is not displayed but whose value is submitted to the server.
image: A graphical submit button. You must use the src attribute to define the source of the image and the alt attribute to define alternative text. You can use the height and width attributes to define the size of the image in pixels.
month: HTML5 A control for entering a month and year, with no time zone.
number: HTML5 A control for entering a number.
password: A single-line text field whose value is obscured. Use the maxlength and minlength attributes to specify the maximum length of the value that can be entered.
radio: A radio button, allowing a single value to be selected out of multiple choices.
range: HTML5 A control for entering a number whose exact value is not important.
reset: A button that resets the contents of the form to default values.
search: HTML5 A single-line text field for entering search strings. Line-breaks are automatically removed from the input value.
submit: A button that submits the form.
tel: HTML5 A control for entering a telephone number.
text: A single-line text field. Line-breaks are automatically removed from the input value.
time: HTML5 A control for entering a time value with no time zone.
url: HTML5 A field for entering a URL.
week: HTML5 A control for entering a date consisting of a week-year number and a week number with no time zone.

 #### 7. How would you explain state to a friend who doesn't know code?

 //Your Answer
 State is an object of a component that is intended to be passed as a prop to the child components

 //Googled Answer
State, in React component, is internal dataset which affects the rendering of the component. To some extent state can be considered as the private data or data model of React components.

 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.


 //Your Answer
Props are intended to be passed from parent component to child component.  


 //Googled Answer
Props and state are related. The state of one component will often become the props of a child component. Props are passed to the child within the render method of the parent as the second argument to React.createElement() or, if you're using JSX, the more familiar tag attributes.Props and state are related. The state of one component will often become the props of a child component. Props are passed to the child within the render method of the parent as the second argument to React.createElement() or, if you're using JSX, the more familiar tag attributes.

#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
n/a - have not started yet  
