# flex-css

_Just-add-classes CSS flexbox_

`shariqueFlex.css` has a bunch of cool flexbox classes for you to use in your projects. Great for galleries, home pages, and general just-add-classes-awesomeness.

### Usage

To use shariqueFlex.css in your website, simply drop the stylesheet into your document's `<head>`, and add any flex classes name in your element. That's it! You've got a CSS flex element. Super!

```html
<head>
  <link rel="stylesheet" href="flex-css.min.css">
</head>
```


### Flex Classes

To use flex in your web page add class 'flex' to the parent element. Use the following below classes as per your requirement.

#### flex
`flex`

#### justify-content
`justify-content-center` | `justify-content-flexStart` | `justify-content-flexEnd`
`justify-content-spaceBetween` | `justify-content-spaceAround` | `justify-content-spaceEvenly`
`justify-content-start` | `justify-content-end` | `justify-content-left` | `justify-content-right`
`justify-content-stretch` | `justify-content-safe` | `justify-content-unsafe`

#### flex wrap
`flex-wrap`   | `flex-nowrap`      | `flex-wrap-reverse`

#### flex basis
<!-- Supported for 2 items 50, 45 ; for 3 items 30 ; for 4 items 24 -->
`flex-basis-auto` | `flex-basis-50` | `flex-basis-45` | `flex-basis-30` | `flex-basis-25`

#### Align Self
`align-self-auto` | `align-self-flexStart` | `align-self-flexEnd` | `align-self-baseline`
`align-self-stretch`

#### Align Items
`align-items-stretch` | `align-items-start` | `align-items-end` `align-items-flexStart`
`align-items-flexEnd` | `align-items-center` | `align-items-safe` | `align-items-unsafe`
`align-items-baseline` | `align-items-selfStart` | `align-items-selfEnd`

#### Align Content
`align-content-spaceEvenly` | `align-content-spaceAround` | `align-content-spaceBetween`
`align-content-start` | `align-content-end` | `align-content-safe` | `align-content-unsafe`
`align-content=flexStart` | `align-content-flexEnd` | `align-content-baseline` | `align-content-center` | `align-content-stretch`

### Cross Browsers Difficulties
Note that that browser support for these values is nuanced. For example, space-between never got support from some versions of Edge, and start/end/left/right aren’t in Chrome yet. MDN has detailed charts. The safest values are flex-start, flex-end, and center.

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
const element =  document.querySelector('.my-element')
element.classList.add('flex', 'justify-content-spaceBetween')
```

## Code of Conduct

This project and everyone participating in it is governed by the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [shariquekhan69.sk@gmail.com](mailto:shariquekhan69.sk@gmail.com).

## Contributing

Pull requests are the way to go here. We only have two rules for submitting a pull request: match the naming convention (camelCase, categorised [flex-basis, justify-cotnent, etc]) and let us see a demo of submitted classes in a [pen](http://codepen.io). That **last one is important**.
