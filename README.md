# CODES_WITH_SOLS

## Q1. https://leetcode.com/problems/majority-element-ii/ (Try to Solve first & then come here for intuition)

### Proof (1):
####                          Proof on if ct > n/3: only 2 elements are possible??? 
####                          Its obvious that more than 2 elements can't have ct > n/3,
####                          As if 2 elements have ct > n/3, total ct of elements (for 2) > 2n/3
####                          So, 3rd element must be < n/3 

### Proof (Maybe):
####                       Need proof on how r we so sure that element having ct > n/3, for sure would be a or b??
####                       wouldn't there be  any case where it would get compensated by others??
####                       Ex: 1 1 1 1 2 3 4 5 6 7 8 (Proof mate)
####                       Observation:
####                       Prolly if u see above example, when at element ''2', ct of '1' is 4, so, for the ct of 1 
####                       to be reduced it needs to wait till element '3' (i.e., cross 2 elements), but why?? 
####                       As initially ct2=0 (when at element '2'), so gets updated at element '2', then next iteration when element is '3',
####                       as it doesn't match '1' or '2', hence both counters decrement, making ct1 (for '1') = 3 (As, 4-1) & ct2(for '2') = 0.
####                       So, after every alternate element, our ct1 decreases (in our example).
####                       So, for total ct1 (i.e., 4), to be reduced to 0, we need to have 8 elements after 1's, which is not possible,
####                       as it would exceed 'n' (i.e., 10 currently) to '12', which would change the majority element ct again!!!!
####                       Hence, by observations, its clear that if its a majority element (as 2 are possible in n/3 case),it would fall under 'a' or 'b'
####                       that we are tracking based on counts.

## Q2. https://leetcode.com/problems/find-the-duplicate-number/ (Try to Solve first & then come here for intuition)
#### Check the diagram with example from https://takeuforward.org/data-structure/find-the-duplicate-in-an-array-of-n1-integers/
#### So, when mapped values to values at corresponding index, it forms a linked list (Refer above link for clear picturizartion)

## Q3. https://leetcode.com/problems/integer-break/
#### DP Solution: https://leetcode.com/problems/integer-break/solutions/2469325/c-recursion-memoization-tabulation-spaceoptimization/
#### Math Solution: Do Dry run for atleast 10 n-values (U sholud figure it out!!!)
