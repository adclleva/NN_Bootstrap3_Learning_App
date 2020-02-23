## there's difference between container-fluid and container 
  containers change with different viewpoints

  container fluid changes sizes according to their parent containers

## Bootstrap has a grid system

  a row can have as many rows with columns size from 1 to 12

  another point is that you get a container
    which then would have a row
      with then would have columns

## Columns
- we assign elements within a row, a column width
- we do this with boostrap classes:
  - col-{size}-{number}
- {size} = the size of the viewport which you are targeting
- {number} = number of columns you want the element to span
- sizes:
  - xs (<768), sm(>=768), md(>=992), lg(>=1200)
- Number of columns
  - any number between 1 and 12

## offestting columns
-an example of offsets
  -col-xs-offset-2
    ! an important note is that when you offset you need to reduce the size of the column as well
    ! right when we get into bigger viewports, you have to reset/remove the offset as well
      and example would be : 
        col-md-offeset-0
   
##  Push & Pull
- this concept can change the placement of the conent when switching the different viewports
  - for example we have this
    col-lg-8 col-lg-push-4
    col-lg-4 col-lg-pull-8
      thus when it gets bigger, the column on the top will move 4 to the right and the column on the bottom   
      will move 8 to the left, hence the push and pull
  - anaother caveat is when you want to push and pull during md size screens, you have to push them back as well and have
    them reset
    - here's an example: 
      col-md-push-6 col-lg-8 col-lg-push-0 
      col-md-pull-6 col-lg-8 col-lg-pull-0 
        this will revert and reset when you go from md to lg screens

  ## Clearfix
  - when there are elements that are off elements to clear the floats
    - you do that by add this code between the elements that are offset
      <div class="clearfix"></div> this bootstrap class will fix the errors
        this is considered a quick fix
  you can also use this css example to fix it as well
  .thumb:nth-child(odd){clear: both;}

## Text styles
- you can use the text styles given from bootstrap
- here's an example below
  - <span class="h3">Header 3</span>
- you can use bootstrap's style classes like lead and other things to overrride the default 

## List Styles
- here are some examples for list styles that bootstrap provides
  list-unstyled
    you can use it for ul, ol, and li
  list-inline    
    this will make it horizontal, good for navigations
    you can use it for ul, ol, and li but not dl
  dl-horizontal 
    makes the dt and dd be next to each other

## Button Styles
- here are some classes that you can apply to the buttons
  - btn 
  - btn-default
  - btn-primary
  - btn-sm
  - active disabled
  - etc. 
- examples
  - <a href="#" class="btn btn-default active">active</a>
  - <button class="btn btn-default" disabled="disabled">button</button> 

## Image Styles
- img-responsive
  - you can give this class for an image to get these styles:
    display: block;
    max-wdith: 100%;
    height: auto;
