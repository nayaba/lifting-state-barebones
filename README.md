# Lifting State - React Shopping Cart

  Objective: Build a React shopping cart app with the following features:

  1. Set up your React app using Vite and configure ESLint rules.
     - Clear out the default `App.jsx` and create a basic setup with "Hello World!".

  2. Plan and implement a component hierarchy for the shopping cart:
     - Create a main `Shop` component and render it in `App.jsx`.
     - Include two reusable `InventoryList` components for Shop and User inventories.

  3. Create an initial data structure:
     - Add the following to src/data/data.js
      ```js
      // src/data/data.js
      export const inventoryData = [
        { _id: 62345, name: 'Banana', price: 0.27 },
        { _id: 22345, name: 'Avocado', price: 2 },
        { _id: 82345, name: 'Yellow Onion', price: 0.5 },
        { _id: 15345, name: 'English Cucumber', price: 1.5 },
        { _id: 12445, name: 'Local Organic Free Range Eggs', price: 6 },
        { _id: 12545, name: 'Milk', price: 2.79 },
        { _id: 12745, name: 'Cauliflower Head', price: 3 },
        { _id: 72345, name: 'Flour Tortillas', price: 3 },
        { _id: 92345, name: 'Butter', price: 4 },
        { _id: 16345, name: 'Cherry Tomatoes', price: 3 },
        { _id: 52345, name: 'Cantaloupe', price: 3.29 },
        { _id: 42345, name: 'Chicken Breast', price: 12 },
        { _id: 32345, name: 'Whole Roasted Chicken', price: 10.99 },
        { _id: 12645, name: 'Ground Beef', price: 9 },
        { _id: 12945, name: 'Pasta Sauce', price: 2.49 },
        { _id: 55555, name: 'Penne Rigate Pasta', price: 1.25 },
        { _id: 13345, name: 'Spaghetti Pasta', price: 2 },
        { _id: 12845, name: 'Ketchup ', price: 3.49 },
        { _id: 19345, name: 'Yellow Mustard', price: 2.19 },
        { _id: 18345, name: 'Mayonnaise', price: 4 },
        { _id: 10002, name: 'Bread', price: 2 },
        { _id: 17345, name: 'Peanut Butter', price: 4.19 },
        { _id: 10001, name: 'Swiss Cheese', price: 3.99 },
        { _id: 85325, name: 'Shredded Mozzarella', price: 4.19 },
        { _id: 14345, name: 'Steelhead Trout Fillet', price: 11.99 },
      ];
      ```
     - Import inventory data into the app.
      ```js
        import { inventoryData } from '../../data/data';
      ```
     - Use `useState` in `Shop` to initialize two arrays:
       - `shopInventory` for store items.
       - `userInventory` for the cart.

  4. Add functionality to transfer items:
     - Allow users to move items from `shopInventory` to `userInventory` by clicking "Add Item".
     - Allow users to move items back by clicking "Remove Item".
     - Use `setState` to update arrays in state immutably.

  5. Pass props and map over data:
     - Use props to pass data and event handlers from `Shop` to `InventoryList`.
     - Dynamically generate list items using `map` and display item names and prices.

  6. Conditionally render buttons:
     - Show "Add Item" for shop inventory and "Remove Item" for user inventory.
     - Use ternary operators to conditionally display the appropriate button.

  7. Style your components:
     - Create separate CSS files for `Shop` and `InventoryList`.
     - Use flexbox to align the inventory lists side by side.

  8. Implement UI improvements:
     - Show a message like "Empty" when an inventory list is empty.
     - Use a ternary operator for conditional rendering.

  Bonus Challenge:
  - Add a feature to calculate and display the total price of items in the user inventory.
  - Add a search bar to filter items in the shop inventory by name.

  References:
  - [React State](https://react.dev/learn/state)
  - [Updating Arrays in State](https://react.dev/learn/updating-arrays-in-state)

