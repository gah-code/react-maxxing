# Fast React Pizza Co. - React Application

![Design preview for the Manage landing page coding challenge](./src/assets/Screen%20Shot%202024-08-20%20at%202.55.07%20PM.png)

This code is a simple React application for a fictional pizza restaurant called **"Fast React Pizza Co."**. It displays a menu of pizzas, including details such as the name, ingredients, price, and whether they are sold out. The app consists of several functional components:

## Components

- **`App`**:  
  The main container for the application, which renders the `Header`, `Menu`, and `Footer` components.

- **`Header`**:  
  Displays the restaurant's name with some basic styling.

- **`Menu`**:  
  Displays the list of available pizzas by mapping over the `pizzaData` array. If there are no pizzas available, a message prompts users to check back later.

- **`Pizza`**:  
  A component for rendering individual pizzas, showing an image, ingredients, and the price. If a pizza is sold out, it displays a "SOLD OUT" message and applies a CSS class to indicate that.

- **`Footer`**:  
  Displays the restaurant's operating hours. If the restaurant is open, it shows an order button; otherwise, it shows a message indicating when the restaurant will be open.

- **`Order`**:  
  Displays the restaurant's operating hours and provides an option for users to place an order.

### Data

The app includes static data in the `pizzaData` array, simulating a list of pizzas with relevant details such as ingredients, prices, photos, and availability.

### Features

- **Dynamic Hours**:  
  The app checks the current time to determine if the restaurant is open or closed and updates the UI accordingly.

- **Responsive Menu**:  
  The menu adapts to the data provided, displaying pizzas or a placeholder message if no items are available.

### Example Data

```javascript
const pizzaData = [
  {
    name: 'Focaccia',
    ingredients: 'Bread with italian olive oil and rosemary',
    price: 6,
    photoName: 'pizzas/focaccia.jpg',
    soldOut: false,
  },
  {
    name: 'Pizza Margherita',
    ingredients: 'Tomato and mozarella',
    price: 10,
    photoName: 'pizzas/margherita.jpg',
    soldOut: false,
  },
  ...
];
```
