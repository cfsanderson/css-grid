# CSS Grid - Course Notes

## 02 - Starter Files and Tooling Setup
## 03 - CSS Grid Fundamentals
## 04 - CSS Grid Dev Tools
## 05 - CSS Grid Implicit vs Explicit Tracks
## 06 - CSS grid-auto-flow Explained

`grid-template-columns: ##px ##px ##px;` this would explicitly layout 3 columns at ## pixels each. The auto keyword can be added to fill remaining space at any interal (e.g. `10px auto 100px`).  

`grid-template-rows` works similarly but for rows  

### implicit vs explicit  
- if you create it = explicit
- if you let the browser create them = implicit
- dashes = implicit rows/columns
- dots = implicit rows/columns
- solid outer lines = explicit start/stop rows/columns

> dev tools > layout tab (can show overlays of explicit, implicit, gap, track numbers, etc.)

`grid-auto-rows` tells browser how to handle any extra rows that are not handled explicitly

## 07 - Sizing tracks in CSS Grid
`auto` works with the widest/tallest element in the column/row respectively - similar to how auto works on a spreadsheet.

## 08 - CSS Grid repeat function

## 09 - Sizing Grid Items
**SUPER cool!**
Use `grid-column: span #;` or `grid-row: span #;` to tell how many of the grid to break over.  

## 10 - Placing Grid Items

## 11 - Spanning and Placing Cardio

## 12 - auto-fit and auto-fill

The difference is in how it takes up space _as it becomes available_ on responsive widths.  
Easy to see in a left-to-right list where the right-most thing is pinned to the right of the page (e.g. `.item { grid-column-end: -1; }`) - not possible with `auto-fit`.

## 13 - Using minmax() for Responsive Grids

## 14 - Grid Template Areas

## 15 - Naming Lines in CSS Grid
The browser numbers lines but you can also give them class-like names to make referring to it in code easier. It is even possible to give them more than one name (e.g. `[content-start site-left]`).

## 16 - grid-auto-flow dense Block Fitting

So cool! 
Able to automoatically fill spaces like a photo gallery.

## 17 - CSS Grid Alignment + Centering

[CSS Tricks guide](https://css-tricks.com/snippets/css/complete-guide-grid/)

## 18 - Re-ordering Grid Items

## 19 - Nesting Grid with Album Layouts

## 20 - CSS Grid Image Gallery

## 21 - Flexbox vs CSS Grid

## 22 - Recreating Codepen

## 23 - Bootstrappy Grid with CSS Variables

## 24 - Responisve Website

## 25 - Full Bleed Blog Layout

