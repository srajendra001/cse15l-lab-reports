# Lab 5
## Part 1
1) **Student**: Can someone help me figure out what's wrong with my `merge` function? I think the bug might related to the second List but I'm not fully sure. Here's a picture of my code for the function as well as the tests that I ran.\
  ![merge function](merge.png)\
  ![test functions](test.png)
2) **TA**: It seems like you're on the right track. Maybe try stopping in the `merge` function and see what's going on using jdb. Also write out what you think should be happening before running the debugger so you can see exactly where the issue is.\
3) **Student**: I noticed that once I completed adding all the elements of `list1`, there was an issue with how I was adding the remaining elements from `list2`. In the debugger I noticed that the `index2` variable wasn't being updated correctly. Additonally, the program kept adding the second element in `list2` to the `result` array since `index2` wasn't being incremented.\
   
