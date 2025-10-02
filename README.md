# Recipe App

This is a simple recipe management application built with **Angular**.  
It allows you to:

- Create and store recipes  
- View and manage a recipe list  
- Create and store a shopping list  

## Features
- **Authentication**: Users can sign up and log in using Firebase Authentication.  
- **Data Storage**: Recipes and shopping list items are stored in Firebase Realtime Database.  

## Important Notes
- This project uses **Firebase** for authentication and data storage.  
- **Firebase configuration data is not included** in this repository for security reasons.  
- To run the project correctly, you must add your own Firebase configuration data inside `src/environments/environment.ts` (and optionally `environment.prod.ts`).  

Example structure for `environment.ts`:

```ts
export const environment = {
  production: false,
  firebase: {
    apiKey: "YOUR_FIREBASE_API_KEY",
    authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
    databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT_ID.appspot.com",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID"
  }
};
