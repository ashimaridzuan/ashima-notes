# Responsive Design Notes

## Responsive Web Design

Responsive web design ensures layouts adapt to different screens and devices.

- Use fluid units like `%`, `vw`, `vh`, and `fr`.
- Combine flexible layouts with media queries.
- Prefer mobile-first development.

## Media Queries

A media query applies styles conditionally.

```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

Common media features:
- `min-width` / `max-width`
- `orientation`
- `aspect-ratio`
- `resolution`
- `hover`
- `pointer`
- `prefers-reduced-motion`

### Breakpoints example

```css
@media (max-width: 600px) {
  .header {
    font-size: 1rem;
  }
}

@media (min-width: 601px) and (max-width: 1024px) {
  .header {
    font-size: 1.5rem;
  }
}

@media (min-width: 1025px) {
  .header {
    font-size: 2rem;
  }
}
```

## Mobile-First Design

Start with styles for small screens and layer in larger breakpoints.

Benefits:
- Better mobile performance
- Cleaner cascade
- Easier progressive enhancement

Example:

```css
.container {
  display: block;
}

@media (min-width: 768px) {
  .container {
    display: flex;
  }
}
```

## Additional Media Features

```css
@media (aspect-ratio: 16/9) {
  .video-container {
    padding: 56.25% 0 0 0;
  }
}

@media (min-resolution: 192dpi) {
  .logo {
    background-image: url('logo-high-res.png');
  }
}

@media (hover: hover) {
  .button {
    cursor: pointer;
  }
}

@media (prefers-reduced-motion: reduce) {
  .animated-element {
    animation: none;
    transition: none;
  }
}
```
