Furthering CSS revision via FreeCodeCamp's CSS Grid resources and copying passed code to Git repo as I go through each task. Documenting below anything new I learn, which will be most of module as I am currently unfamiliar with grid.

- Learned to create initial grid with columns and rows.
    - Initiated by diplay:grid.
    - Add rows or columns with grid-template-columns / grid-template-rows. Values are given one after the other, not comma separated.
        - Shorthand is to use repeat(iterations, size), e.g. grid-template-columns:repeat(100, 20px) woul give 100 columns at 20px.

- Learned to create a column or row gap with grid-column-gap / grid-row-gap. Takes a size value.
    - Shorthand grid-gap: a b (optional);
        - If only one value given, applies to both rows and columns. If two given, applies first to rows, second to columns.

- Learned to control spacing on columns and rows.
    - Property grid-column and grid-row, takes 2 values, indicating the lines of the grid as which the coolumn/row must start or end. Example:
    grid-column: 1 / 4; will make the column span the first three columns (between lines 1 to 4).

- Learned to align grid items with justify and align properties.
    - Can align per item with justify-self / align-self (declared on item), or all items with justify-items / align-items (on grid container).
        - Takes values of start, center or end.

- Learned to create grid areas, assigning multiple cells to an area or splitting into their own.
    - Method one:
        Created with grid-template-areas. Properties given individually in quotation marks, each indicating a row and containing a value for each column within the row. Example (3 x 3 grid):

            grid-template-areas:
            "header header header"
            "advert content content"
            "footer footer footer";
            
        Top row will become one single cell spanning three columns, likewise with footer. Middle row becomes split across 2 areas; 'advert' and 'content', taking 1 column and 2 columns respectively.
    
    - Method two:
        Done on the fly by giving start and end properties based on lines of the grid in the format:
        
        grid-area: horizontal line to start at / vertical line to start at / horizontal line to end at / vertical line to end at;

        Example:

        grid-area: 1/2/2/4;

        Would span area between first-to-second horizontal lines and second-to-fourth vertical lines (in a 4 x 4 grid this would be top row, second and third cells).