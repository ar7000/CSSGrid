Furthering CSS revision via FreeCodeCamp's CSS Grid resources and copying passed code to Git repo as I go through each task. Documenting below anything new I learn, which will be most of module as I am currently unfamiliar with grid.

- Learned to create initial grid with columns and rows.
    - Initiated by diplay:grid.
    - Add rows or columns with grid-template-columns / grid-template-rows. Values are given one after the other, not comma separated.

- Learned to create a column or row gap with grid-column-gap / grid-row-gap. Takes a size value.
    - Shorthand grid-gap: a b (optional);
        - If only one value given, applies to both rows and columns. If two given, applies first to rows, second to columns.

- Learned to control spacing on columns and rows.
    - Property grid-column and grid-row, takes 2 values, indicating the lines of the grid as which the coolumn/row must start or end. Example:
    grid-column: 1 / 4; will make the column span the first three columns (between lines 1 to 4).

- Learned to align grid items with justify and align properties.
    - Can align per item with justify-self / align-self (declared on item), or all items with justify-items / align-items (on grid container).
        - Takes values of start, center or end.