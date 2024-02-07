[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
    1. Asymptotic analysis doesn't take into account constant factors. So while the constant factors do take time to run or memory to store, they aren't analysed. 
    2. Asymptotic analysis doesn't take into account for the uniqueness of different implementations, for example some implemetations might use less memory than others and while this doesn't change anything for the asymptotic analysis it can effect actual run time of algorithms.
    3. Differences in hardware will also affect actual performance.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  Guess: I would guess that it will take around 65 seconds. Because, 1000*log(1000) = 3000 and 10000*log(10000) = 40000  40000/3000 = 13.3333333  40000 is about 13 times larger than 1000  so 5 seconds * 13 = 65 seconds

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. a larger binary tree requires more memory and that could possibly slow things down.
  2. Maybe the hardware i use to measure the actual run time is slower, so it slows the process down.
  3. Maybe the implimentation of a binary search isn't as optimized as it could be so it is slowed down.

Add your answers to this markdown file.
