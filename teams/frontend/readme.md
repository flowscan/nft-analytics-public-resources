# Front-end 

TODO

## Typescript 

We're using TypeScript for our project, so we would need this analytics project to use TypeScript so that we can easily expand / modify it in the future whenever needed.

## API Client 

We're using [Apollo](https://www.apollographql.com/) for the GraphQL client. There's an example of our API usage on `./examples/graphql.tsx` as a reference. 

## CSS & Design

At Flowscan we're using [Tailwind](https://tailwindcss.com/), so it would be nice if you can use the same UI framework with ours. 

For cards, we're using these Tailwind CSS classes: `rounded-xl overflow-hidden p-6 bg-white`, with an additional `card-shadow` custom class for the shadow. The specification for `card-shadow` is: 
```css
.card-shadow {
    box-shadow: 0 0 35px rgba(127,174,150,.15);
}
```

### Colors 

The background of our site is pure white `#FFFFFF` or `bg-white` in Tailwind, however for tabbed layouts such as https://flowscan.org/contract/A.0b2a3299cc857e29.TopShot, the background for the tab content is `bg-gray-50`.

For most of the text content, we're using plain black (`text-black`). Accent colors are using a variation of `text-green-500`.

## Icons 

We're using [Feathericons](https://feathericons.com/) for most part of the icons. Although feel free to use an external icon if needed.

## Fonts 

We're using [TT Commons](https://typetype.org/fonts/tt-commons/) as the default type-face for the website (we have a web-font license for it). As a fallback, we're using [Inter](https://fonts.google.com/specimen/Inter) from Google Fonts.

Feel free to use a mix of them for the analytics interface. 
