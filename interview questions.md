## 1. What are media queries?

Media queries allow you to apply CSS styles conditionally based on the **device's characteristics**, like width, height, resolution, or orientation.

```css
@media (max-width: 768px) {
  body { font-size: 14px; }
}
```

## 2. Explain mobile-first vs desktop-first CSS design

* **Mobile-first:** Start designing for small screens first, then use media queries to adapt to larger screens.
* **Desktop-first:** Start with desktop styles, then use media queries to adapt to smaller screens.

> Mobile-first is preferred because it ensures better performance and usability on small devices.

## 3. How do you test responsiveness?

* Use **browser DevTools** (Device Toolbar) to simulate different screen sizes.
* Resize the browser window manually.
* Test on real devices if possible.
* Tools like **Responsively App** or online simulators can help.

## 4. What units are best for responsive layouts?

* **Relative units:** `em`, `rem`, `%`, `vw`, `vh`
* Avoid fixed units like `px` for widths and font sizes where possible.

## 5. What is viewport meta tag?

The viewport meta tag controls how a page is scaled on mobile devices:

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

## 6. How does flexbox help in responsive design?

Flexbox allows **flexible alignment and distribution** of elements in a container.

* Can reorder elements with `flex-direction` and `order`.
* Supports flexible sizing with `flex-grow` and `flex-shrink`.
* Works well for **one-dimensional layouts** (row or column).

## 7. Difference between absolute and relative units?

* **Absolute units:** `px`, `pt` – fixed size, not responsive.
* **Relative units:** `%`, `em`, `rem`, `vw`, `vh` – adapt to parent/container or viewport, ideal for responsive design.

## 8. How to handle images in responsive design?

* Use **max-width: 100%** and height: auto:

```css
img { max-width: 100%; height: auto; }
```

* Use **`<picture>` element** for different resolutions.
* Optimize images for mobile to reduce load times.

## 9. What is adaptive vs responsive design?

* **Responsive:** Layout adjusts fluidly to any screen size.
* **Adaptive:** Layout uses predefined breakpoints for specific screen widths.

## 10. Explain CSS grid responsiveness

CSS Grid allows **two-dimensional layouts** (rows and columns) to adapt:

```css
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
}
```

* `auto-fit` and `minmax()` create flexible columns.
* Works well for galleries, cards, and complex layouts.
