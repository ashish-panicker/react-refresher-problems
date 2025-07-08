# Learn React - Coding CHallanges

### **Beginner Problems (Focus on Basics, Attributes, and Expressions)**

1.  **Basic Greeting Component:**
    * Create a component called `Greeting`.
    * It should render an `<h1>` tag that says "Hello, World!"

2.  **Dynamic Greeting:**
    * Modify the `Greeting` component (or create a new `DynamicGreeting`).
    * It should accept a `name` prop.
    * Render an `<h1>` that says "Hello, [name]!" (e.g., "Hello, Alice!").
    * Test it with different names from your `App.js`.

3.  **Simple Product Card:**
    * Create a component called `ProductCard`.
    * It should accept `productName`, `price`, and `imageUrl` props.
    * Render a `div` with an `<h2>` for the product name, a `<p>` for the price, and an `<img>` tag for the image.
    * Make sure to include an `alt` attribute for the image.

4.  **Button with Dynamic Text and Event:**
    * Create a component called `MyButton`.
    * It should accept a `text` prop for the button's label.
    * It should accept an `onClick` prop (a function).
    * Render a `<button>` with the dynamic `text`.
    * Attach the `onClick` function to the button's `onClick` event.
    * In `App.js`, render two `MyButton` instances, each with different text and a simple `alert()` function for `onClick`.

5.  **Conditional Message:**
    * Create a component called `LoginStatus`.
    * It should accept an `isLoggedIn` boolean prop.
    * If `isLoggedIn` is true, render a `<p>` tag that says "Welcome back!".
    * If `isLoggedIn` is false, render a `<p>` tag that says "Please log in to continue.". (Use the ternary operator or logical `&&`).

---

### **Intermediate Problems (Focus on Lists, Styling, and Children Prop)**

6.  **Shopping List:**
    * Create a component called `ShoppingList`.
    * It should accept a `items` prop, which is an array of strings (e.g., `['Milk', 'Eggs', 'Bread']`).
    * Render an `<ul>` list.
    * Use `map()` to iterate over the `items` array and render each item as an `<li>`.
    * **Crucial:** Remember to add a unique `key` prop to each `<li>`.

7.  **Styled Component:**
    * Create a component called `StyledBox`.
    * It should accept `backgroundColor` and `textColor` props.
    * Render a `div` that uses inline styles to set its background color and text color based on the props.
    * Add some padding and a border radius to the `div` as well.
    * Inside the `div`, render a `<p>` tag with some dummy text.

8.  **Card with Children:**
    * Create a component called `Card`.
    * It should accept a `title` prop (string) and use the `children` prop.
    * Render a `div` with an `<h2>` for the title and then render the `children` prop below the title.
    * Apply some basic inline styles to the `Card` `div` (e.g., border, padding).
    * In `App.js`, render several `Card` components, each containing different JSX content (e.g., a paragraph, an image, a list).

9.  **User Profile Display:**
    * Create a component called `UserProfile`.
    * It should accept a `user` prop, which is an object with properties like `firstName`, `lastName`, `age`, `email`, and `isAdmin` (boolean).
    * Display the user's full name (`firstName lastName`), age, and email in separate `<p>` tags.
    * Conditionally display a `<span>` that says "(Admin)" next to the name if `isAdmin` is true.

---

### **Advanced Problems (Combining Concepts, Spread Props)**

10. **Interactive Counter:**
    * Create a component called `Counter`.
    * It should display a number (`count`). Start with `0`. (You'll eventually use `useState` for this, but for now, just render a fixed number).
    * Include two buttons: "Increment" and "Decrement".
    * When "Increment" is clicked, the `count` should increase.
    * When "Decrement" is clicked, the `count` should decrease.
    * **(Hint: This is where you'll first truly need React's `useState` hook. If you haven't learned it yet, just focus on setting up the buttons and showing a static number for now, or consider it a stretch goal after learning `useState`).**

11. **Dynamic Button Group:**
    * Create a component called `ButtonGroup`.
    * It should accept a `buttonsData` prop, which is an array of objects. Each object should have `id`, `label`, and `onClick` (function) properties.
    * Use `map()` to render a `MyButton` component (from problem #4) for each item in `buttonsData`.
    * Use the spread operator (`...`) to pass all relevant properties from `buttonsData` objects to the `MyButton` component.
    * In `App.js`, define an array of button data and pass it to `ButtonGroup`.

12. **Alert Box with Different Types:**
    * Create a component called `AlertBox`.
    * It should accept `message` (string) and `type` (string: "success", "warning", "error") props.
    * Based on the `type` prop, apply different inline styles (e.g., green background for success, yellow for warning, red for error).
    * Render the `message` inside the alert box.
    * (Optional: Add a close button that conditionally renders the alert based on an internal state - this would require `useState`).

---

**How to approach these problems:**

1.  **Read the problem carefully.** Understand what the component needs to do and what props it will receive.
2.  **Start with the basic JSX structure.** Get the static HTML-like elements in place.
3.  **Introduce props.** Use curly braces `{}` to embed JavaScript variables and expressions.
4.  **Implement logic.** Add conditional rendering, mapping over arrays, or event handlers.
5.  **Test thoroughly.** Check your `App.js` to ensure the components render correctly and behave as expected.
6.  **Refactor (optional but good practice):** Once it's working, see if you can make your code cleaner, more readable, or more efficient.
