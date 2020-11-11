# React Native

## Step 3 - Styling

> 📘 View React Native's - [Style documentation](https://reactnative.dev/docs/style)

### Task 1 - Layout

Create a new card component showing an image on at the top and a heading below. The heading and image should have the same width.

```
Image: /assets/yeezy-infants.png
Heading text: Yeezy 700 V3 Infants Safflower
```

### Task 2 - Layout 2

Without changing the HTML in Task 1, change the layout so that the image is on the left, and the heading is to its right.

### Task 3

Vertically center the heading text to the image.

### Task 4

Add a 1px black border to the card outline. Make the borders rounded by 5px.

### Task 5

Add description text below the heading. Add a scroll region to the card body and set the card body height to 100px.

```
Description:
A new colorway of the popular Adidas Yeezy 700 V3 is hitting shelves this week.

The sportswear giant confirmed across its social media platforms that the “Safflower” colorway of the Kanye West-designed lifestyle sneaker is releasing globally this Saturday. However, fans in North America will have to wait until January to buy a pair.

The lifestyle runner is dressed in a white-based Primeknit upper that’s contrasted by yellow stripes running across the sides, while a white TPU shell wraps the knitted material. Adding to the look is a black neoprene tongue and sock liner. Instead of the responsive Boost cushioning that was used on the V1 and V2 versions of the Yeezy 700, the V3 variation opts for EVA foam cushioning instead.

Fans in North America will be able to pick up a pair at Adidas.com/Yeezy, the Confirmed app and at select Yeezy stockists on Jan. 16, 2021. The shoe will come with a $200 price tag.
```

### Task 4

Set a dynamic max-height for the card, which is 300px shorter than screen height in portrait mode or 100px shorter than screen height in landscape mode.

### Task 6 - StyleSheet

Duplicate to create a second card with hard coded property values. DRY up the styles between them so styles reference the same StyleSheet.

```
Image: /assets/superstar-infants.png
Heading text: Superstar Infants Classic
Description:
Pro players swore by them. Hip hop legends wrote songs about them. And everybody still loves them. These infants' adidas Superstar Shoes show off the same classic lines as the first pairs in the '70s. Strap closures take the place of laces for easy on and off.

The adidas Superstar was first released in 1970 as the first sneaker of its kind. At a time when basketball shoes were mostly made from canvas, Superstar used cowhide upper for comfort and durability. Later adidas began testing a rubber toe cap on different silhouettes to reinforce the shoe's upper.

First used on the Tennis silhouette, the rubber toe cap was redesigned to become the shell toe - now an iconic detail of Superstar. The Superstar was also the first leather basketball shoe: and now nearly 50 years later, the adidas Superstar still lives up to its hype. The masses took this silhouette from the court to the streets - and made Superstar an icon.

Arguably the most recognisable and iconic adidas sneaker, the adidas Superstar has been a mainstay of street fashion and culture through a number of generations. These iconic shell toe kicks cut a distinguished silhouette and enjoy a unique basketball heritage. From sports to the streets: the adidas Superstar sneaker rose in prominence with the birth of hip-hop and streetwear culture. The world witnessed Superstar transition to a lifestyle staple - leading to its ultimate icon status.
```

> 📘 View React Native's - [Stylesheet](https://reactnative.dev/docs/stylesheet)

### Task 5 - theme

Create a file called "theme" to contain design tokens. Include tokens that among others, include a primary colour, and a large font size.

Add a button below the description text "Buy presale" and use the design token to assign values to style property.
