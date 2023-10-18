[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11799895&assignment_repo_type=AssignmentRepo)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
- We might not be considering the power of the system and the system specs (hardware constraints)
- Ignoring the constant C factor
- 
- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  -The average run time to traverse a binary search tree is log2(n) so for the timing of the first element its log2(1000) = 9.966, if we do the same for the second at 10000 entries
  that would be log2(10000) = 13.288, to get the rate of growth that would just be the ratio between those two values, so 13.288/9.966 which is 1.33 repeating. If in reality the function took 5 seconds instead of the 9.966, we would just multiply that 5 seconds by the growth rate to estimate the timing of 10000, so 5 * 1.33 which equals 6.66 repeating. So approximately 7 seconds 
  

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.
  I mean we could just explain that maybe the hardware is off? Ram got overloaded or something trying to search that many elements.
  Maybe there's another factor in this data structure, its not balanced or something of the like.

Add your answers to this markdown file.
