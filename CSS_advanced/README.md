# Web Development Starter Guide

This starter guide provides essential information for web developers, covering various aspects of HTML and CSS.

## Table of Contents

1. [Selectors, Properties, and Values](#selectors-properties-and-values)
2. [Block and Inline Styling](#block-and-inline-styling)
3. [Ensuring Consistency Across Browsers (CSS Reset)](#ensuring-consistency-across-browsers-css-reset)
4. [Setting up CSS Variables](#setting-up-css-variables)
5. [Differences Between Inline, Embedded, and External CSS](#differences-between-inline-embedded-and-external-css)
6. [How Grid Systems Work (with Floats)](#how-grid-systems-work-with-floats)
7. [Differences Between Icons Webfonts and SVG Icons](#differences-between-icons-webfonts-and-svg-icons)
8. [Differences Between Pseudo-Classes and Pseudo-Elements](#differences-between-pseudo-classes-and-pseudo-elements)
9. [How to Make Background Gradients](#how-to-make-background-gradients)
10. [How to Animate Elements in CSS](#how-to-animate-elements-in-css)
11. [How to Transform (2D, 3D) Elements](#how-to-transform-2d-3d-elements)
12. [What Vendor Prefixes Are](#what-vendor-prefixes-are)

## 1. Selectors, Properties, and Values

- **Selectors:** Patterns used to select HTML elements based on type, class, ID, or attributes.
  
- **Properties:** Styles applied to selected elements, determining visual aspects like color, size, and font.
  
- **Values:** Assigned to properties to define how styles should be applied (e.g., color: "red" or "#FF0000").

## 2. Block and Inline Styling

- **Block Styling:** Creates a block on the page, stacking on new lines, taking up the full width.
  
- **Inline Styling:** Flows within content, doesn't start on new lines, only takes up necessary width.

## 3. Ensuring Consistency Across Browsers (CSS Reset)

A CSS reset is essential to standardize default styles across different browsers, preventing inconsistencies.

## 4. Setting up CSS Variables

CSS variables, defined with `--` prefix, are declared in the `:root` selector to be globally available.

## 5. Differences Between Inline, Embedded, and External CSS

- **Inline CSS:** Applied directly to an HTML element using the `style` attribute.
  
- **Embedded CSS:** Placed within the `<style>` tag in the HTML document's head.
  
- **External CSS:** Stored in a separate CSS file and linked to the HTML document using the `<link>` tag.

## 6. How Grid Systems Work (with Floats)

Grid systems help create layouts by dividing the page into columns and rows. Floats, historically used for layout, can be problematic and are mitigated by grid systems.

## 7. Differences Between Icons Webfonts and SVG Icons

- **Icon Webfonts:** Included as a font, styled with CSS, scalable, and offer performance advantages.
  
- **SVG Icons:** Created using Scalable Vector Graphics, resolution-independent, easily manipulated with CSS and JavaScript.

## 8. Differences Between Pseudo-Classes and Pseudo-Elements

- **Pseudo-Classes:** Select and style elements based on state or position (e.g., `:hover` or `:nth-child()`).
  
- **Pseudo-Elements:** Select and style parts of an element (e.g., `::before` or `::after`), adding content before or after the actual content.

## 9. How to Make Background Gradients

Use the `background` property with `linear-gradient` or `radial-gradient` functions. Example: `background: linear-gradient(to right, #ff7e5f, #feb47b);`

## 10. How to Animate Elements in CSS

Define animations with `@keyframes` and apply them with the `animation` property. Example:

```css
@keyframes slide {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(100px);
  }
}

.element {
  animation: slide 2s infinite;
}
