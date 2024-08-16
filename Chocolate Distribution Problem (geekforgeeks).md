**Chocolate Distribution Problem**

CODE

![image](https://github.com/user-attachments/assets/4e9e8997-60c1-495e-9ae2-fb2ffa913665)

EXPLANATION

First we sort the array using the sort function, with this we get the minimum difference between each packets of chocolate.

After sorting the array, we select the sliding window of size M among the array, and for each window, we take the difference of elements at each end, which gives the difference between the min and max number of chocolates given.

KEEP A NOTE:
The iteration in i stores the end of the sliding window instead of the start, and j starts at the 0th element.

Along witht the above sliding, we assign a very large number to the final value that is to be returned, and as we slide to each window, we compare final's value with the diff in the number of min and max chocolates given.

If final is greater than the diff, then replace the final with the diff.

Then finally return final.
