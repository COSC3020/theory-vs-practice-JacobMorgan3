[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
    1. Asymptotic analysis doesn't take into account constant factors. So while the constant factors do take time to run or memory to store, they aren't analysed. 
    2. Asymptotic analysis looks at the growth rate as the input increases, but for small input sizes one algorithm might be better than another even though it's asymptotic analysis suggests otherwise. For example some implementations of merge/quick sort use insertion sort for small arrays. They do this because the growth rate of $n^2$ grows slower than $lg(n)$ with small inputs, but as n increases $lg(n)$ over takes $n^2$
    3. Differences in hardware will also affect actual performance. The numebr of processes the cpu can do per cycle can speed up run time or slow it down. The speed of memory is also a consideration, fast memory will help. In addition, not having enough memory to do the whole sort in memory will also slow things down. 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

Guess: We know that the complexity of a binary search tree is $log(n)$. $log_2(1000) = 9.9$ $log_2(9000) = 13$ this grows by about half of the original, so finding the same element in the binary search tree would take about 8 seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. A larger binary tree requires more memory, getting all that memory into caches when it is needed may slow things down.
  2. Maybe the hardware I have is operating slower than normal (slower than it could be), because of this it took longer to find the element than expected.
  3. Maybe the implimentation of a binary search isn't as optimized as it could be so it is slowed down.

Add your answers to this markdown file.
