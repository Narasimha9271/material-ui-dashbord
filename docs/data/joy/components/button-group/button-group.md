---
product: joy-ui
title: React Button Group component
components: Button, IconButton, ButtonGroup
githubLabel: 'component: ButtonGroup'
---

# Button Group

<p class="description">The Button Group combines a set of related buttons.</p>

{{"component": "modules/components/ComponentLinkHeader.js"}}

## Introduction

The Button Group component combines a set of buttons that have similar or related functionality.

{{"demo": "ButtonGroupUsage.js", "hideToolbar": true, "bg": "gradient"}}

## Basics

The Button Group component can wrap [`Button`](/joy-ui/react-button/) and [`IconButton`](/joy-ui/react-button/#icon-button).

{{"demo": "BasicButtonGroup.js"}}

## Customization

### Variants

The Button Group component supports Joy UI's four [global variants](/joy-ui/main-features/global-variants/): `outlined` (default), `solid`, `soft`, and `plain`.

{{"demo": "VariantButtonGroup.js"}}

:::info
To learn how to add your own variants, check out [Themed components—Extend variants](/joy-ui/customization/themed-components/#extend-variants).
Note that you lose the global variants when you add custom variants.
:::

### Sizes

The Button Group component comes in three sizes: `sm`, `md` (default), and `lg`.

{{"demo": "GroupSizesColors.js"}}

:::info
To learn how to add custom sizes to the component, check out [Themed components—Extend sizes](/joy-ui/customization/themed-components/#extend-sizes).
:::

### Colors

Every palette included in the theme is available via the `color` prop.
Play around combining different colors with different variants.

{{"demo": "ButtonGroupColors.js"}}

### Disabled

Use the `disabled` prop to disable all the buttons.
Note that if you explicitly specify the `disabled` prop on the buttons directly, it will override what is used in the Button Group.

{{"demo": "DisabledButtonGroup.js"}}

### Detached

Use the `detached` prop to separate buttons from each other.
It will remove the border radius override.

{{"demo": "DetachedButtonGroup.js"}}

### Vertical group

The Button Group component can be displayed vertically using the `orientation="horizontal"` prop.
Note that this prop has no effect on `IconButton` component.

{{"demo": "GroupOrientation.js"}}

### Stretching button

Use the `buttonFlex` prop to make the buttons fill the available space of the Button Group component.

{{"demo": "FlexButtonGroup.js"}}

#### Minimum width

For a large container, control the default width of the buttons by providing a valid [CSS `flex`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex) value to the `buttonFlex` prop.

{{"demo": "MinWidthButtonGroup.js"}}

### Split button

The Button Group component can also be used to create a split button.
The dropdown can change the button action (as in this example) or be used to immediately trigger a related action.

{{"demo": "SplitButton.js"}}

### Separator color

When the Button Group's variant is <b>not</b> `outlined`, separators are created between buttons.
To control the color of the separator, override the CSS variable `--ButtonGroup-separatorColor` via the `sx` prop.

{{"demo": "SeparatorButtonGroup.js"}}

## Using it with a Tooltip

The Button Group component supports arbitrary children that wrap the buttons by preserving the same appearance.

{{"demo": "TooltipButtonGroup.js"}}

## Common examples

### Pill button group

Use the CSS variable `--ButtonGroup-radius` to control the radius of the start and end buttons.

{{"demo": "RadiusButtonGroup.js"}}

### Custom separator

This example uses the `Divider` component to create a custom separator between the buttons.
The CSS variable `--ButtonGroup-separatorColor` is then set with an arbitrary value to remove the default separator.

{{"demo": "CustomSeparatorButtonGroup.js"}}
