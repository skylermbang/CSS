CSS Flexible layout box 

-2.1 
    Before flex box : 
    by default : display set to block so they dont want anything beside
    inline <-> block  
    but inline has no width and height 
    so we have inline-block

    but the problem is this is not mobile screen friendly and human have to calculate everything. on each screen it was very imperative 

    flexboxes are very declarative 


-2.2 

    For responsive and declarative , we use flexbox
    no need to hardcode the value of the margine values.

    you talk to the parent containers 

    justify-content : move thing horizontally  // space-around , center , space-between
  


-2.3

  gap : all the child will have distance between eachother
  default property : felx-direct : row; 
  * the default flex-direction : row (horizontal)


 -2.4 

  flex lay out have two axis :  main axis ;  cross-axis   the position of the axis are depend on the flex-direction


  when flex-direction : row  
   
   main axis :  horizontal
   croass axis :   vertical
                 


-2.7
 .box*20>{$}  to make 20
 default behavior :  flex box try to show everything in one row by ignoring the width of the flex contents
 we have to  use  flex-wrap: wrap it control the flex box is multiline or single line
 flex-flow : row  wrap   : specify the flex-direction row and flex-wrap : wrap 