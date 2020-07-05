# CSS Grid - Course Notes

`grid-template-columns: ##px ##px ##px;` this would explicitly layout 3 columns at ## pixels each. The auto keyword can be added to fill remaining space at any interal (e.g. `10px auto 100px`). 

`grid-template-rows` works similarly but for rows

## implicit vs explicit  
- if you create it = explicit
- if you let the browser create them = implicit
- dashes = implicit rows/columns
- dots = implicit rows/columns
- solid outer lines = explicit start/stop rows/columns

> dev tools > layout tab (can show overlays of explicit, implicit, gap, track numbers, etc.)
