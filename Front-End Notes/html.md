# HTML Notes

## Semantic HTML

- Semantic HTML uses tags that describe meaning, such as `header`, `nav`, `section`, `article`, `aside`, and `footer`.
- Benefits:
  - Code readability
  - SEO improvement
  - Better accessibility
  - Future-proof structure
  - Easier team collaboration

## Void Elements

Void elements cannot contain content or closing tags.

Examples:
- `br`
- `hr`
- `img`
- `input`
- `meta`
- `link`

## List Elements

- `ul` + `li`: unordered list
- `ol` + `li`: ordered list
- `ol start="5"`: begin numbering from 5

Example:
```html
<ol start="5">
  <li>Item one</li>
  <li>Item two</li>
</ol>
```

## File Paths

- `./` refers to the same folder.
- `../` refers to one folder up.

## HTML Boilerplate

A standard HTML document includes:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document</title>
</head>
<body>
  <!-- Content goes here -->
</body>
</html>
```
