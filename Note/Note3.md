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



span :

you can easily specify the how many row/columns for this 
grid-row : span 2  = grid-row: 1 / -1;   t

