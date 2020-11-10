# React Native

## Step 1 - Platform Components

React Native has a different document object model, and so has its own native components. For example, in React Native, there is no such thing as a `<div>` element, instead you would use `<View>`. Similarly, there is no `<a>`, rather we can use `<Button>` or other Touchable components. Similarly, there is no '<p>', rather we can use '<Text>".

Under the hood, React Native's Components internally map to iOS or Android native elements.

> 📘 View React Native's - [Component reference](https://reactnative.dev/docs/components-and-apis)

### Task 1

Create a blue button with the text "View".

[TODO: insert picture - button]

### Task 2

Create a blue button with the text "View" and add the Right Chevron image alongside the text inside the button.

Blue colour: #0fc7fa

[TODO: insert picture - button with image]

### Task 3

Create a card component with a card body and card footer.

The card body should include a title, description and image. Add the button created to the card footer.

Title: Adicolor T-Shirt
Description:  
adidas Originals' 'Adicolor' range is inspired by the label's rich heritage and incorporates signature branding, like the Trefoil logo that's been around since 1972.
Image: /assets/adicolor-tshirt

[TODO: insert picture - card component with button footer]

### Task 5

Add a second card, and use [`<FlatList>`](https://reactnative.dev/docs/flatlist) to inject data via props.

Title: Adilette Slides
Description:  
First introduced in 1972, the adilette has since risen to global prominence as the most popular slide ever. Built for recreation and relaxation, this lightweight style features a secure jelly bandage and a contour footbed for long lasting comfort.
Image: /assets/adicolor-tshirt

### Task 6

Tapping the button should navigate to Google.

Url: https://www.google.com.au/?search={%PRODUCT_NAME%}

### Task 7

If the user taps anywhere on the card, navigate the user to Google.
