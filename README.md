# flex-css

_Just-add-classes CSS flexbox_

`flex-css` has a bunch of cool flexbox classes for you to use in your projects. Great for galleries, home pages, and general just-add-classes-awesomeness.

### Usage

To use flex-css in your website, simply drop the stylesheet into your document's `<head>`, and add any flex class name to your element.

```html
<head>
  <link rel="stylesheet" href="flex-css.min.css">
</head>
```


### Flex Classes

Add class `flex` to the parent element, then combine with any of the classes below.

#### display
`flex` | `inline-flex`

#### justify-content
`justify-content-center` | `justify-content-flexStart` | `justify-content-flexEnd`
`justify-content-spaceBetween` | `justify-content-spaceAround` | `justify-content-spaceEvenly`
`justify-content-start` | `justify-content-end` | `justify-content-left` | `justify-content-right`
`justify-content-stretch` | `justify-content-safe` | `justify-content-unsafe`

#### flex-wrap
`flex-wrap` | `flex-nowrap` | `flex-wrap-reverse`

#### flex-basis
<!-- Supported for 2 items: 50, 45 | for 3 items: 33, 30 | for 4 items: 25 | full width: 100 | reset: 0, auto -->
`flex-basis-auto` | `flex-basis-0` | `flex-basis-25` | `flex-basis-30` | `flex-basis-33` | `flex-basis-45` | `flex-basis-50` | `flex-basis-100`

#### flex-grow
`flex-grow-0` | `flex-grow-1` | `flex-grow-2` | `flex-grow-3`

#### flex-shrink
`flex-shrink-0` | `flex-shrink-1` | `flex-shrink-2` | `flex-shrink-3`

#### flex-flow
`flex-flow-row-wrap` | `flex-flow-row-nowrap` | `flex-flow-row-wrapReverse`
`flex-flow-column-wrap` | `flex-flow-column-nowrap` | `flex-flow-column-wrapReverse`

#### flex-direction
`flex-direction-row` | `flex-direction-rowReverse`
`flex-direction-column` | `flex-direction-columnReverse`
`flex-direction-inherit` | `flex-direction-initial` | `flex-direction-unset`

#### order
`order-0` | `order-1` | `order-2` | `order-3` | `order-4` | `order-5`
`order-first` | `order-last`

#### align-self
`align-self-auto` | `align-self-normal` | `align-self-start` | `align-self-end`
`align-self-flexStart` | `align-self-flexEnd` | `align-self-center`
`align-self-baseline` | `align-self-selfStart` | `align-self-selfEnd` | `align-self-stretch`

#### align-items
`align-items-normal` | `align-items-start` | `align-items-end`
`align-items-flexStart` | `align-items-flexEnd` | `align-items-center`
`align-items-baseline` | `align-items-selfStart` | `align-items-selfEnd`
`align-items-stretch` | `align-items-safe` | `align-items-unsafe`

#### align-content
`align-content-normal` | `align-content-start` | `align-content-end`
`align-content-flexStart` | `align-content-flexEnd` | `align-content-center`
`align-content-baseline` | `align-content-stretch`
`align-content-spaceBetween` | `align-content-spaceAround` | `align-content-spaceEvenly`
`align-content-safe` | `align-content-unsafe`

### Cross Browser Notes
Browser support for some values is nuanced. For example, `space-between` never got support from some versions of Edge, and `start`/`end`/`left`/`right` aren't in Chrome yet. MDN has detailed compatibility charts. The safest values are `flex-start`, `flex-end`, and `center`.

Full example:

```html
<div class="flex justify-content-spaceAround flex-wrap">
  <div class="flex-basis-45">
    content....
  </div>
  <div class="flex-basis-45">
    content....
  </div>
</div>
```

It's possible to overwrite the css of the class by adding inline, internal or external css as shown below.

> [!NOTE]
> Your class element should come after the flex-css class.

```css
.yourElement {
 flex-basis: 35%;
}
```
```html
<div class="flex-basis-45 yourElement">
```

## Usage with Javascript

You can add or remove css classes with Javascript. A simple example:

```javascript
const element = document.querySelector('.my-element')
element.classList.add('flex', 'justify-content-spaceBetween')
```

## Code of Conduct

This project and everyone participating in it is governed by the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [shariquekhan69.sk@gmail.com](mailto:shariquekhan69.sk@gmail.com).

## Contributing

Pull requests are the way to go here. We only have two rules for submitting a pull request: match the naming convention (property-value, categorised [flex-basis, justify-content, etc]) and let us see a demo of submitted classes in a [pen](http://codepen.io). That **last one is important**.

[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/shariquekhan1997/flex-css)
