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

- `justify-*` aligns with the row (x) axis
- `align-*` aligns with the column (y) axis

Each uses either `start`, `end`, `stretch`, or `center`

- `justify-content`
- `align-content`


## 18 - Re-ordering Grid Items

```css
.container {
  display: grid;
  grid-gap: 20px;
  grid-template-columns: repeat(10, 1fr);
}

.content {
  grid-column: 1 / -1;  
  order: 3;
}

.logo {
  grid-column: span 2;
  order: 2;
}

.nav {
  grid-column: span 8;
  order: 1;
}

@media (max-width: 700px) {
  .content {
    grid-column: 1 / -1;  
    order: 3;
  }

  .logo {
    grid-column: 1 / -1;  
    order: 1;
  }

  .nav {
    grid-column: 1 / -1;  
    order: 2;
  }
}
```

## 19 - Nesting Grid with Album Layouts
I did a little overachieving with this one. This creates an album layout with a left side "featured" list that is a little bit bigger.

```css
.all__albums {
      display: flex;
      flex-direction: row;
    }
    .albums1 {
      width: 20%;
      padding: 0 50px 0 0;

    }

    .alb {
      background: rgba(255, 255, 255, 0.9);
      color: rgba(255, 255, 255, 0.9);
      padding: 0 0 20px 0;
      margin: 0 0 20px 0;
    }

    .alb .album__artwork { 
      width: 100%;
      padding: 0 0 10px 0;
    } 

    .alb .album__details {
      padding: 10px;
      color: rgba(0, 0, 0, 0.85);
    }

    .albums2 {
      display: grid;
      grid-gap: 20px;
      grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    }

    .album {
      color: white;
      background: rgba(255, 255, 255, 0.2);
      box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
      padding: 20px;
      display: grid;
      grid-template-columns: 150px 1fr;
      align-items: center;
      grid-gap: 20px;
    }

    .album__artwork {
      width: 100%;
    }
```

## 20 - CSS Grid Image Gallery


## 21 - Flexbox vs CSS Grid

## 22 - Recreating Codepen

## 23 - Bootstrappy Grid with CSS Variables

## 24 - Responisve Website

## 25 - Full Bleed Blog Layout

