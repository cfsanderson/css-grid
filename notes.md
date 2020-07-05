# CSS Grid - Course Notes

## 01-06

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

## 07
`auto` works with the widest/tallest element in the column/row respectively - similar to how auto works on a spreadsheet.

## 08

## 09
**SUPER cool!**
Use `grid-column: span #;` or `grid-row: span #;` to tell how many of the grid to break over.  


