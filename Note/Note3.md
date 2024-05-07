Lecture 3  CSS Grid 

Flexbox : control main-axis 

Grid :  Can control both row and column you 


give this to father : 
  grid-template-columns: 100px 200px 50px;
  grid-template-rows: 200px 100px;

give tjos to child :
  grid-row-start: 1 ;
  grid-row-end: -1;
  grid-row: 1 / -1;


fr-unit :
   similar to the flex-grow  1fr  1:1:1:1 also work in responsivly
   grid-template-columns: 1fr 1fr 1fr 1fr ; 
   grid-template-rows: 1fr 1fr 1fr;

grid-template-areas: : 
    grid-template-columns: 1fr 1fr 1fr 1fr ; 
    grid-template-rows: 1fr 2fr 1fr;
    grid-template-areas: "header header header header"
                        "menu content content content" 
                        "footer footer footer footer";
    


    make it easiser : 
    grid-template: "header header header header"  1fr 
                 "menu content content content" 2fr 
                 "footer footer footer footer" 0.5fr /1fr 1fr 1fr 1fr    


3.5
    span :
        you can easily specify the how many row/columns for this 
        grid-row : span 2  = grid-row: 1 / -1;   t


3.6 Auto Columns and Rows
    For dynamic contents
    these two properties will add the 
    "unexpected" contents size and in row (default)
    grid-auto-rows: 1fr;   /* incase of any extra  rows added*/
    grid-auto-flow: row 


3.7 Align and Justify Items 

    Justify-items : stretch the contents in width
    stretch only works when the child dosent have any width

    Align-items : strech only work when we dont have height

3.8 Align and Justify 

    place the whole grid thing 
    this will only works when the grid container have extra space (usually when the grid cell is set with px not fr measurment)

    short-cut :  place-content : center start;


3.9 Auto Sizing and Minmax

    grid-template-columns: 1fr max-content 1fr;

    max-content : as big as the content can be
    min-content : as small as longerst words 

    grid-template-columns: 1fr minmax(min-content,1fr) 1fr;
  

3.10 Auto Fill and Auto Fit

    responsive grid 

    3grids (web) -> 2 grids(ipad) -> 1grid (mobile)

      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr))
       
       auto-fill and auto-fit  
       auto-fill:   as many column you create even if it 1fr 
                        create empty column in the extra space

       auto-fit:  empty column will be ignored
                        grid continers collapse the empty space