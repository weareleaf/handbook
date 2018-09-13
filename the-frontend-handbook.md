# The Frontend Handbook

## Table of Contents

* [Welcome](#welcome)
* ~~HTML~~
* [CSS](#css)
* ~~JavaScript~~
* ~~File structure~~
* ~~Boilerplates~~

## Welcome

Anyone with a little knowhow and determination can make a website, but crafting scalable and manageable design systems are a different kettle of fish. The Frontend Handbook is intended to help align our team, keeping our standards consistent, and mitigating as many common pitfalls as we can.

## CSS

We use CSS extensively as part of our day-to-day, and while it's easy to pick-up, it can quickly become problematic at scale. We can't change the language or it's pitfalls, but by following our internal conventions for writing CSS, we can work towards creating more maintainable, readable, and scalable systems.

### SCSS

Preprocessing our CSS helps us create scalable and modular design systems, and we use [Sass][1] (or more specifically SCSS) to extend our powers with nesting, imports, and mixins.

### General principles

A consistent codebase feels like a clean and familiar codebase. By creating a standard set of guidelines on how we structure and format our CSS, we allow ourselves to move between projects without having to learn a new set of rules each time.

- Follow agreed and existing conventions religiously.
- Don't prematurely optimise; strive for clarity and readability.
- Use 2 spaces for code indentation, rather than tabs.
- Keep line-lengths to 80 characters in your code editor.
- Place comments on the line above their intended context.

#### Format

- Place each selector on its own line.
- Include a space between the selector and the opening brace.
- Include a space, after the colon, between a property and value.
- Use single quotes, rather than double or no quotes
- Omit the unit when specifying a value of 0
- Omit leading 0's when writing fractions
- Include a space after each comma in comma-separated value.

```
.input,
.input[type='text'],
.input[type='email'] {
	background: linear-gradient(#eee, rgba(255, 255, 255, .25));
	border: solid rgba(0, 0, 0, .75);
	margin: 0;
}
```

##### SCSS
- Place `@extend` statements at the start of a declaration.
- Place `@include` statements after any `@extend` statements.
- Only extend placeholder selectors.

```
.label {
	@extend %h5;
	@include clearfix;
	@include padding-vertical(.5em);
	@include truncate;
}
```

### BEM

Each and every components should follow the [Block Element Modifier (BEM)][2] methodology. BEM is a powerful naming convention, written specifically with reusability and modularity in mind, that helps keep our code readable, robust, and consistent.   

#### Block

A block is the outermost part of a component, providing context and scope.

#### Element

Any children within a block are known an elements. Elements are prefixed with two underscores `__`

#### Modifier

Modifiers are used to manipulate the default state of a block. Modifiers are prefixed with two hyphens `--`

```scss
// Block
.alert { ... }

// Element
.alert__heading { ... }
.alert__message { ... }

// Modifier
.alert--success { ... }
.alert--warning { ... }
```

### Property order

CSS Properties should always be written in alphabetical order, top to bottom. Many developers favour [ordering properties into predetermined groups][3], but having the `height` and `width` properties a few lines closer hardly seems worth the excess congestive load.

Alphabetic ordering instantly proscribes where a property should be added, and allows us to scan for the presence of a property in an existing component.

### Nesting

Try not to nest more than 3 levels deep. If you find yourself going further, it's often an indication that the component in question may be in need of a restructure.

```scss
// Don't
.alert {

  &__header {

    &__title {

      &__icon {

        &--inverted {

        }
      }
    }
  }
}
```

### Colors

When denoting color using hexadecimal notation, use all lowercase letters. Both three-digit and six-digit hexadecimal notations are absolutely fine; if you can specify a color using three-digit notation, you should.

```scss
// Do
color: #ccc;
color: #eff0f2;

// Don't
color: #333333;
color: #EEE;
```

Note too that when referencing color within the context of CSS, we always use the American spelling, even outside of code itself.

#### IDs

The `ID` attribute is incredibly useful, acting as a scripting hook for JavaScript, providing an association between labels and form elements, and anchoring users to specific parts of a web page. However, `ID`s should never been used as CSS selectors.

IDs carry a higher specificity than classes, causing inevitable pain (often to some other poor soul) when used within a design system.

#### Naming classes

It sounds ridiculous, but naming things is one of the hardest things you'll encounter in your day-to-day.

Try and use names that are as succinct as possible, but not to the detriment of clarity.

Consider not only the proposed usage, but the possible usage of the component. Make decisions, especially when naming, that promote reusability and modularity.

Finally, always use hyphens should connect multiple words.

```scss
// Do
.nav { ... }
.page-header { ... }

// Don't
.navigation_bar { ... }
.pHead { ... }
```

### Units

CSS provides us with several units for expressing sizes, and it's important to know when to use each (and which ones to steer clear of altogether).

#### Ems

Ems are sized relative to the elements within which they're used, and as such, are useful in any instances where we need control over the scale of a specific area.

A good use-case for `em` is an icon used inside a `button`, where the icon's size should relate to the button's text size.

#### Rems

Rems are scalable unit, relative to the `html` elements `font-size`. Any scalable sizing that doesn't require an `em` should use `rem`.

#### Percentages

Percentages are relative to the width and height of a parent element, and are incredible useful when you need to span either some of all of the available space.  

#### Pixels

Pixels are usually best avoided due to their hard-coded, disproportional nature. However, that can be valuable in instances where you may actually want that inflexibility.

`Border-width` is a good example of a property you may actually not want its value to change as the interface scales either up or down.

#### Viewport units

The viewport is the area where the browser renders its content, and both Viewport Width (`vw`) and Viewport Height (`vh`) are relative to the size of the 'browser window'.

Viewport units are useful when creating full-screen sections, such as login pages, or hero-banners.

#### Unitless

Finally, a unitless `line-height` (e.g. `1.4`) is considered best practice, acting as a multiplier of the `font-size` value.

```scss
// Do
border-width: 1px;
font-size: 1.2rem;
Height: 100vh;
Line-height: 1.25;
Padding: 1em;
width: 100%;

// Don't
font-size: 14pt;
width: 24cm;
```

#### Component structure

The ordering of classes should considered when created or updating a component. As the complexity of a component increases, finding specific styles becomes a lot harder.

Rather than simply tagging new styles to the bottom of the file,  considered their importance and order within the component hierarchy.

```scss
// Do
.modal {

  &__header { ... }
  &__body { ... }
	&__footer { ... }
}

// Don't
.modal {

  &__header { ... }
  &__footer { ... }
  &__body { ... }
}
```

[1]: https://sass-lang.com/
[2]: http://getbem.com/
[3]: https://9elements.com/css-rule-order/
