# Grid Reference

CSS grid layout or CSS grid is a technique in Cascading Style Sheets that allows web developers to create complex responsive web design layouts more easily and consistently across browsers. There have been other methods for controlling web page layout methods, such as tables, the box model, and CSS flex box. CSS grid is currently not an official standard (it is a W3C Candidate Recommendation) although it has been adopted by most major browsers. [Wikipedia](https://en.wikipedia.org/wiki/CSS_grid_layout)



## container

### display

Establishes a new grid formatting context for children.

```css
display: grid; 
display: inline-grid; 
display: subgrid;
```

### grid-template

Defines the rows and columns of the grid.

```css
grid-template-columns: 12px 12px 12px;
grid-template-rows: 12px 12px 12px; 
grid-template-columns: repeat(3, 12px);
grid-template-rows: repeat(3, auto); 
grid-template-columns: 8px auto 8px;
grid-template-rows: 8px auto 12px; 
grid-template-columns: 22% 22% auto;
grid-template-rows: 22% auto 22%;
```

### grid-gap

Specifies the size of column and row gutters.

```css
grid-row-gap: 1px;
grid-column-gap: 9px; 
grid-gap: 1px 9px; 
grid-gap: 6px;
```

### justify-items

Aligns content in a grid item along the row axis.

```css
justify-items: start; 
justify-items: end; 
justify-items: center; 
justify-items: stretch; (default)
```

### align-items

Aligns content in a grid item along the column axis.

```css
align-items: start; 
align-items: end; 
align-items: center; 
align-items: stretch; (default)
```

### justify-content

Justifies all grid content on row axis when total grid size is smaller than container.

```css
justify-content: start; 
justify-content: end; 
justify-content: center; 
justify-content: stretch; 
justify-content: space-around; 
justify-content: space-between; 
justify-content: space-evenly;
```

### align-content

Justifies all grid content on column axis when total grid size is smaller than container.

```css
align-content: start; 
align-content: end; 
align-content: center; 
align-content: stretch; 
align-content: space-around; 
align-content: space-between; 
align-content: space-evenly;
```

### grid-auto-flow

Algorithm for automatically placing grid items that aren't explicitly placed.

```css
grid-auto-flow: row; 
grid-auto-flow: column; 
grid-auto-flow: dense;
```

## children

### grid-column

Determines an items column-based location within the grid.

```css
grid-column-start: 1;
grid-column-end: 3; 
grid-column-start: span 3; 
grid-column-start: 2;
grid-column-end: 4; 
grid-column: 2 / 3 
grid-column: 2 / span 2
```

### grid-row

Determines an items row-based location within the grid.

```css
grid-row-start: 1;
grid-row-end: 3; 
grid-row-start: span 3; 
grid-row-start: 2;
grid-row-end: 4; 
grid-row: 1 / 3; 
grid-row: 1 / span 3;
```

### grid-row + grid-column

Combining grid rows with grid columns.

```css
grid-row: 1 / span 2;
grid-column: 1 / span 2; 
grid-row: 2 / span 2;
grid-column: 2 / span 2;
```

### justify-self

Aligns content for a specific grid item along the row axis.

```css
justify-self: start; 
justify-self: end; 
justify-self: center; 
justify-self: stretch; (default)
```

### align-self

Aligns content for a specific grid item along the column axis.

```css
align-self: start; 
align-self: end; 
align-self: center; 
align-self: stretch; (default)
```

This markdown was created from [grid.malven.co](http://grid.malven.co/) as reference