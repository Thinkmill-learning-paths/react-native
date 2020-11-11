# React Native

## Step 6 - Plugins - Data management

> Recommended reading - [Foundation 2 - Key differences to Web](@todo - link)

> 📘 React Native docs - [Security](https://reactnative.dev/docs/security)

### Task 1 - App wide state

Create a project with some basic routing set up using React Navigation.

Default routes: Home (/)
Route: Success (/success)

On Home route, show text at the top of the screen saying "Welcome %firstName %lastName." If firstName or lastName as undefined, instead say "Welcome friend". Below, create a form with a submit button and inputs for first name and last name fields.

On Success route, show a back link "Back to home". Below, display text "Success! You saved your name as %firstName %lastName."

App flow requirements:

- Starting from Home, text displays "Welcome friend"
- When the user submits the form, the app should navigate to the Success page and show the name displayed.
- Typing in fields should not update the welcome text.
- Form can not be submitted with empty fields.
- When the user navigates from Success back to Home, text should display "Welcome %firstName %lastName".
- Force closing the app and then reopening should reset welcome text and display "Welcome friend"

### Task 2 - Persisted state

Our intention now is the edit the example, so that when a user force closes and reopens the app, that the data does not reset.

Install [AsyncStorage](https://react-native-async-storage.github.io/async-storage/docs/install/) and use it's API to persist data across sessions.

Validate this works manually, then try deleting the data via Phone Settings and validate that "Welcome friend" resets.
