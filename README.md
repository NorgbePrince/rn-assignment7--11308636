# rn-assignment7--11308636

## Fakestore

### Overview

---

Fakestore is a straightforward e-commerce mobile application developed with React Native. It enables users to browse a list of products obtained from an external API, view detailed information about each product, add products to their cart, and manage the cart's content. The app employs AsyncStorage to locally store selected items on the device.

### Features

---

#### HomeScreen

Displays a list of available products fetched from an external API, each with an "Add to Cart" button.

#### ProductDetailScreen

Provides detailed information about a selected product.

#### CartScreen

Shows items added to the cart, allowing users to remove items as needed.

#### Drawer Navigation

Facilitates easy navigation with a drawer menu accessible via a button or swipe gesture.

#### Data Storage

Utilizes AsyncStorage to store and retrieve cart items locally.

### Design Choices

#### User Experience

The app emphasizes a simple and intuitive user experience. The product list is presented in a grid format for easy browsing, with each product card displaying an image, title, and price for quick access to key information.

#### Navigation

React Navigation is used to handle screen transitions. A stack navigator is employed for the main screens (Home, Product Detail, Cart), and a drawer navigator is implemented for additional navigation options.

#### State Management

React's `useState` and `useEffect` hooks are used for state management and handling side effects, simplifying data flow and enhancing code maintainability.

#### Local Storage

AsyncStorage is used for persistent data storage, ensuring that cart data is retained even if the app is closed or the device is restarted. AsyncStorage is chosen for its simplicity and ease of integration with React Native.

### Data Storage Implementation

#### AsyncStorage

Cart items are stored locally using AsyncStorage. When an item is added to the cart, the app retrieves the current cart from AsyncStorage, updates it with the new item, and saves it back. Similarly, when an item is removed, the stored cart is updated accordingly.

#### Data Retrieval

On app startup, cart data is loaded from AsyncStorage to restore the user's cart state. An asynchronous function reads the cart data from storage and updates the app's state.

### Usage

---

- **HomeScreen:** Browse products and add them to the cart.
- **ProductDetailScreen:** View detailed product information by tapping on it in the HomeScreen.
- **CartScreen:** View and manage items in the cart.
- **Drawer Navigation:** Access additional navigation options via the drawer menu.

### Setup

---

1. Clone the repository.
2. Install dependencies using `npm install` or `yarn install`.
3. Run the app on a simulator or physical device using `npx react-native run-android` or `npx react-native run-ios`.

### Conclusion

This project showcases the creation of a basic e-commerce mobile app with React Native, featuring product browsing, detailed product views, and cart management. It highlights the use of React Native components and hooks, as well as the integration of AsyncStorage for persistent local storage.

### Screenshots
![](/Fakestore/images/photo_2024-07-11_17-19-28.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-30.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-31.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-33.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-43.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-44.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-46.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-47.jpg)
![](/Fakestore/images/photo_2024-07-11_17-19-50.jpg)