# Gridd
CSS Grid Framework pre-built with IE 10+ compatibility

Breakpoints are same one used for frameworks such as [Tachyons](https://tachyons.io/)

This is an additional framework that exclusively utilizes CSS grid to produce layouts. This is especcially efective on creating header/menu layouts or for creating uniquely declared layouts for web projects. This also works great as an addition to any frameworks you may be already using. I use this alongside Tachyons just add in another tool for more direct uses.

This can also be combined with stylesheets if you need to create extra specific layouts or to declare items in "area" cells the style declarations for grid template areas and grid template are as such:

`.grid-stuff {
  grid-template: "one two three";
  grid-template-areas: "one two three";
}
.grid-item {
  grid-cell: "one";
  grid-area: one;
}`
The above portion utilizes the current spec for grid-template-areas and the 2011 spec for IE10 grid cell

All styles are applied as HTML classes keeping with the concept of layout in HTML and styles separate in our stylesheets.
The sytax is as follows:

### Basic grid declaration
`<div class="grid"></div>`

### Prebuilt grid dimensions
`<div class="grid2x2"></div>`  
`<div class="grid3x3"></div>`  
`<div class="grid4x4"></div>`  
`<div class="grid12x12"></div>`  

### Custom grid dimensions
`<div class="grid grid-cols-3 grid-rows2"></div>`

### Custom grid layout with various breakpoints
`<div class="grid grid-cols-4-l grid-rows-2-l grid-cols-1 grid-rows-8"></div>`

### Declaring sub-items inside grid cells for a 12x12 grid
`<div class="u-col-2 u-row-1"></div>`

### Declaring sub-items inside grid cells for a 12x12 grid at breakpoints
`<div class="u-col-2-l u-row-1-l u-col-5-m u-row-2-m u-col-1 u-row-8"></div>`
