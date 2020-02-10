# learn-vue

Challenges from https://www.vuemastery.com/courses/intro-to-vue-js/

## Challenge 1

- How to begin writing a Vue application with a Vue instance, and how to load basic data onto the webpage.
- The Vue instance is the root of every Vue application
- The Vue instance plugs into an element in the DOM
- The Vue instance’s data can be displayed using the mustache-like syntax {{ }} called an expression.
- Vue is reactive

## Challenge 2 - Attribute Binding

- Data can be bound to HTML attributes.
- Syntax is v-bind: or : for short.
- The attribute name that comes after the : specifies the attribute we’re binding data to.
- Inside the attribute’s quotes, we reference the data we’re binding to.

## Challenge 3 - Conditional Rendering

- There are Vue directives to conditionally render elements:
  - v-if
  - v-else-if
  - v-else
  - v-show
- If whatever is inside the directive’s quotes is truthy, the element will display.
- You can use expressions inside the directive’s quotes.
- V-show only toggles visibility, it does not insert or remove the element from the DOM.


## Challenge 4 - List Rendering

- The v-for directive allows us to iterate over an array to display data.
- We use an alias for the element in the array being iterated on, and specify the name of the array we are looping through. Ex: v-for="item in items"
- We can loop over an array of objects and use dot notation to display values from the objects.
- When using v-for it is recommended to give each rendered element its own unique key.

## Challenge 5 - Event Handling

- The v-on directive is used to allow elements to listen for events
- The shorthand for v-on is @
- You can specify the type of event to listen for:
  - click
  - mouseover
  - any other DOM event
- The v-on directive can trigger a method
- Triggered methods can take in arguments
- *this* refers to the current Vue instance’s data as well as other methods declared inside the instance

## Challenge 6 - Class & Style Binding

- Data can be bound to an element’s style attribute
- Data can be bound to an element’s class
- We can use expressions inside an element’s class binding to evaluate whether a class should appear or not

## Challenge 7 - Computed Properties

- Computed properties calculate a value rather than store a value.
- Computed properties can use data from your app to calculate its values.
- Computed properties are cached. Cache is updated when parts of the calculation are changed. 
- You should not be mutating your data model from within a computed property.

## Challenge 8 - Components

[Video](https://www.vuemastery.com/courses/intro-to-vue-js/components)

[Further information on templates](https://medium.com/js-dojo/7-ways-to-define-a-component-template-in-vuejs-c04e0c72900d)

- Components are blocks of code, grouped together within a custom element
- Components make applications more manageable by breaking up the whole into reusuable parts that have their own structure and behavior
- **Data on a component must be a function**
- Props are used to pass data from parent to child
- We can specify requirements for the props a component is receiving
- Props are fed into a component through a custom attribute
- Props can be dynamically bound to the parent’s data
- Vue dev tools provide helpful insight about your components
