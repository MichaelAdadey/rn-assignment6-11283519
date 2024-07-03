# rn-assignment6-11283519

# React Native E-Commerce App

## Overview

This React Native application provides a simple e-commerce experience where users can browse products on the home screen and add them to their cart. The cart is accessible from the home screen and allows users to view and remove items, as well as see the total estimated price.

## Design Choices

### Component Structure

- **HomeScreen**: Displays a list of products that users can browse. Each product has an image, name, description, price, and an "add to cart" button.
- **CartScreen**: Displays the items added to the cart, allowing users to view details, remove items, and see the total estimated price. Also provides a button to navigate back to the home screen.

### State Management

- **useState**: Used to manage local state for cart items in both `HomeScreen` and `CartScreen`.
- **useEffect**: Used to load cart items from AsyncStorage when the components are mounted.

### Navigation

- **react-navigation**: Used to handle navigation between `HomeScreen` and `CartScreen`.

### Data Storage

- **AsyncStorage**: Used to persist cart data between app sessions. This ensures that the cart's state is maintained even if the app is closed and reopened.

## Implementation Details

### HomeScreen

- **Products List**: A predefined list of products is displayed. Each product has an "add to cart" button.
- **Adding to Cart**: When the "add to cart" button is pressed, the product is added to the cart state and saved to AsyncStorage.

### CartScreen

- **Loading Cart**: When the component mounts, it loads the cart data from AsyncStorage into the state.

- **Removing from Cart**: When the remove button is pressed, the product is removed from the cart state and the updated cart is saved to AsyncStorage.

- **Calculating Total Price**: The total price is calculated by summing up the prices of all items in the cart.

### Styles

- **Styling**: Basic styling is applied using `StyleSheet` to ensure a clean and readable interface. This includes layout, typography, and button styles.

![screenshots](<my-app/assets/localhost_8081_(Samsung Galaxy S20 Ultra) (1).png>)
![screenshot](<my-app/assets/localhost_8081_(Samsung Galaxy S20 Ultra).png>)
