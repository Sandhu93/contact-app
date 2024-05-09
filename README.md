# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## src Directory Overview

### assets:

Contains all the static files like images, icons, and global stylesheets. The images subdirectory is specifically for storing image files that will be used across the app.
└───assets
└───images

### components:

Houses reusable UI components such as buttons, input fields, and cards. Components in this folder can be imported and used in multiple places throughout the app.

### constants:

This folder is for storing constant values that are used across the app. This could include configuration values, API endpoints, or any other fixed values that need to be reused.

### containers:

Contains components that are usually connected to the state in some way and serve as containers for other components. These might include page layouts or components that fetch and contain data for their child components.

### context:

Used for state management with React's Context API. It can contain subfolders for actions, initial states, and reducers:
actions: Holds files that define action types and action creators for context state management.
initialstates: Contains files that define the initial state for different contexts used within the app.
reducers: Stores reducer functions that handle state changes based on actions.

### helpers:

Includes utility functions and helper methods that can be used across the app to perform common tasks like formatting dates, filtering data, etc.

### layout:

Contains layout components that define the structural layout of pages (e.g., header, footer, side navigation). These components are used to maintain a consistent layout across the app.

### routes:

Manages the routing of the app. It includes the definition of route paths and the association of those paths with the corresponding view components. This folder typically contains a main router file that uses React Router (or another routing library) to render different pages based on the URL.

### utils:

Similar to helpers, but often contains more generic utilities that can be used project-wide, such as functions for API calls, data transformation functions, and more complex logic that doesn't fit into the helpers category.
