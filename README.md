# CODES_WITH_SOLS

### https://leetcode.com/problems/majority-element-ii/
### Proof (Maybe):
####                      Need proof on how r we so sure that ele having 
####                       ct > n/3, for sure would be a or b??
####                       wouldn't there be  any case where it would get compensated by others??
####                       1 1 1 1 2 3 4 5 6 7 8 (Proof mate)
####                       Observation:
####                       Prolly if u see above example, from element:2, for the ct of 1 
####                       to be reduced it needs to wait till 3 (i.e., 2 elements), as 
####                       initially ct2=0, so gets updated, then next case when val!=a or b,
####                       then gets decremented, 
####                       So, say when n=10, and this would be the worse case, where
####                       ct of '1' is 4, but even there r 6 elements to process, the ct would
####                       reduce only by 3, ensuring it stays as majority element
