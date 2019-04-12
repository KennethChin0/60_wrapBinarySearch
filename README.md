# exercise the List.indexOf

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48

# Inverse functions and logarithms
 y = log2x is the inverse of exponential functions. 
 The graph looks like a curve that starts out steep and flattens out.
 
# Recursive Solution
0. Find which half of the list the desired value is in.
1. decision: if low > high or if list_iAS.get(currentIndex) == findMe (non recursive case)
2. base case: if list_iAS.get(currentIndex) == findMe, return currentIndex
              if low > high, return -1
3. No combination
   Solution to recursive abstraction: (if (list_iAS.get(currentPage) < findMe) return indexOfRecursively(findMe, currentIndex + 1, high);
   Leftover processing: indexOfRecursively(findMe, low, currentIndex -1);
