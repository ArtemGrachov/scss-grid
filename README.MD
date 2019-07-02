# SCSS-grid

Simple SCSS grid generator

## Usage 

Insert `grid` mixin into your code:

```

$breakpoints: (
    sm: 576px,
    md: 768px,
    lg: 992px,
    xl: 1200px
);

@include grid(12, 20px, $breakpoints);

@include grid(4, 5px, $breakpoints, 'zzzz-');
```

## Arguments:

* **$columnsCount** - columns count;
* **$columnGap** - space between columns (default value: `0`);
* **$breakpoints** - breakpoints for media queries, SCSS map (default value: `()`);
* **$prefix** - prefix to be added to row and column classes (e.g. `.zzzz-row`, `.zzzz-col-md-6`; default value: `''`);
* **$colName** -  (e.g. with value 'column' you'll get classes like `.column-sm-5`; default value: `'col'`);
* **$rowName** - row class name (behives like `colName`; default value: `'row'`)

## Offsets, aligns etc.
...weren't included.