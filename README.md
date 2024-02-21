[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
    1. Asymptotic analysis doesn't take into account constant factors. So while the constant factors do take time to run or memory to store, they aren't analysed. 
    2. Asymptotic analysis looks at the growth rate as the input increases, but for small input sizes one algorithm might be better than another even though it's asymptotic analysis suggests otherwise. Because of recussive call overhead or other factors.
    3. Differences in hardware will also affect actual performance. The numebr of processes the cpu can do per cycle can speed up run time or slow it down. The speed of memory is also a consideration, fast memory will help. In addition, not having enough memory to do the whole sort in memory will also slow things down. I'm not certain how multiprocessing would affect asymptotic analysis, but i think it would have no affect. The function doesn't change and the analysis is algorithm in the function not on how the hardware ran it. 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

Guess: We know that the complexity of a binary search tree is $log(n)$. $log_2(1000) = 9.97$ $log_2(9000) = 13.14$ this grows by 1.318 original, so finding the same element in the binary search tree would take about 6.59 seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. Maybe I am running other programs on my computer so more of the cpu and memory are being used for other tasks, so the binary search tree is left with less computing power, so it is slower.
  2. Perhaps the 'search tree' with 10000 elements is not a binary search tree, but some other type. so it has a slower time complexity than a binary search tree.
  3. Perhaps the search tree with 10000 elements is running in the worse case, so a time complexity of $nlog(n)$ which would slow it down.

Add your answers to this markdown file.
