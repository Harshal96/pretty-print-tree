# pretty-print-tree
A simple java function to pretty print a binary tree:

Example:
       1
   2       3
 4   5   6   7
8 9 A B C D E F

In that tree, the number of levels is 4. The spacing at the last level is 1 whereas the indent is 0. You'll get the following values:

level 1:
  indent = 7: (2(4-1) - 1 = 23 - 1 = 8 - 1 = 7)
  first level, so spacing doesn't matter
level 2:
  indent = 3: (2(4-2) - 1 = 22 - 1 = 4 - 1 = 3)
  spacing = 7 (2(4-1) - 1 = 23 - 1 = 8 - 1 = 7)
level 3:
  indent = 1: (2(4-3) - 1 = 21 - 1 = 2 - 1 = 1)
  spacing = 3 (2(4-2) - 1 = 22 - 1 = 4 - 1 = 3)
level 4:
  indent = 0: (2(4-4) - 1 = 20 - 1 = 1 - 1 = 0)
  spacing = 1: (2(4-3) - 1 = 21 - 1 = 2 - 1 = 1)

Note that at the last level you'll always have spacing 1 * element width. Thus for a maximum element width of 3 (e.g. 3-digit numbers) you'd have a spacing of 3 at the last level, in order to get some pretty alignment of the upper levels.
