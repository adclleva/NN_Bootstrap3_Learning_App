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