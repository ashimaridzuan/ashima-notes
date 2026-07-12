# CSS Notes

## CSS Positioning

1. `position: static`
   - Default value
   - Element follows normal document flow

2. `position: relative`
   - Positioned relative to normal location
   - `top`, `right`, `bottom`, `left` move the element without removing it from flow

3. `position: absolute`
   - Positioned relative to the nearest positioned ancestor
   - Removed from normal flow

4. `position: fixed`
   - Positioned relative to viewport
   - Stays fixed while scrolling

5. `position: sticky`
   - Behaves like `relative` until threshold is reached
   - Then becomes fixed

```css
.element {
  position: sticky;
  top: 0;
}
```

## Float and Clear

- `float: left` or `float: right` positions elements and allows text to wrap around them.
- Floated elements are removed from normal flow.

```css
.column-left {
  float: left;
  width: 45%;
}

.column-right {
  float: right;
  width: 45%;
}
```

### Clearfix

A clearfix keeps the parent container around floated children.

```css
.clearfix::after {
  content: "";
  display: table;
  clear: both;
}
```

## Flexbox

- `display: flex` makes a container a flexbox.
- `justify-content` controls main-axis alignment.
- `align-items` controls cross-axis alignment.
- `gap` controls spacing between items.

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}
```

### Flex direction and wrap

- `flex-direction: row | column | row-reverse | column-reverse`
- `flex-wrap: nowrap | wrap | wrap-reverse`

```css
.container {
  display: flex;
  flex-flow: row wrap;
}
```

## CSS Grid

- `display: grid` creates a grid container.
- `grid-template-columns` and `grid-template-rows` define the layout.
- `fr` units distribute available space.

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
}
```

### Alignment

- `justify-items` and `align-items` for cell alignment
- `justify-self` and `align-self` for individual items
