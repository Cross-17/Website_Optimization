## WebWebsite Optimization

###Introduction
This is the 6th projrct of FEND in Udacity, which is to opitimize the performance of a website.

###How to start
Open index.html in any browser to view opitimized website.

###What Optimization I have done
####PageSpeed Score
In this section I simply inline all possible css,js,and image file into index.html, and delete the fond style link. PageSpeed give me 99/100 on both mobile and desktop.

####Scrolling Optimization
This opimization happens in the function updatePositions() resides in main.js.

Frist of all I move the layout query out from the loop, which would eliminate the forced synchronous layout.

Then I replace the item[i].style.left with item[i].style.transform, which eliminates the unnesserary painting

####Resize Optimization
This optimization happens in the function changePizzaSizes(size).

Here I move the layout query out from the loop to eliminate the forced synchronous layout.