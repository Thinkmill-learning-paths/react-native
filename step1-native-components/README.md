# React Native

## Step 1 - Platform Components

> 📘 React Native docs - [Components](https://reactnative.dev/docs/components-and-apis)

### Task 1 - Button

Create a blue button with text "View".

> 📘 React Native docs - [Button](https://reactnative.dev/docs/button)

```
Blue colour: #0fc7fa
```

### Task 2 - Button with icon

Duplicate the button from Task 1 and add a right chevron image icon to the right-hand side of the button text.

```
Image: /assets/chevron-right.png
```

### Task 3 - Card with button

Create a card component with a card body and card footer.

The card body should include a title, description and image.

In the card footer include the button created.

```
Title: Adicolor T-Shirt
Description:
adidas Originals' 'Adicolor' range is inspired by the label's rich heritage and incorporates signature branding, like the Trefoil logo that's been around since 1972.
Image: /assets/adicolor-tshirt
SKU: 111
Category: Clothing
```

### Task 4 - Listview

Add a second card. This time use `<FlatList>` to hoist the data in to a wrapping component and inject data via props.

> 📘 React Native docs - [Flatlist](https://reactnative.dev/docs/flatlist)

```
Title: Adilette Slides
Description:
First introduced in 1972, the adilette has since risen to global prominence as the most popular slide ever. Built for recreation and relaxation, this lightweight style features a secure jelly bandage and a contour footbed for long lasting comfort.
Image: /assets/adicolor-tshirt
SKU: 222
Category: Footwear
```

### Task 5 - Listview 2

Convert `<FlatList>` into `<SectionList>`, and separate items by category. Use the category name to label sections.

> 📘 React Native docs - [SectionList](https://reactnative.dev/docs/sectionlist)

```
Categories: Clothing, Footwear
```

### Task 6 - Button action

Tapping the button should `console.log` the item's SKU.

> 📘 React Native docs - [Debugging](https://reactnative.dev/docs/debugging)

### Task 7 - Non-button action

Tapping the title should `console.log` the item's title text.

### Task 8 - Non-button action 2

Tapping the image should `console.log` the item's SKU.

On tap show visual feedback by making the image fade in opacity slightly.

### Task 8 - Alert and debugging

> 📘 React Native docs - [Alert](https://reactnative.dev/docs/alert)

Add a link to the card footer that says "Quick add". On tap, the link should open an `<Alert />` component with text "Do you want to quick add to cart?" with buttons "Cancel" and "Add".

On tapping "Cancel", dismiss the Alert. On tapping "Add", `console.log` "Added \$PRODUCT_NAME success", and then dismiss the Alert.
