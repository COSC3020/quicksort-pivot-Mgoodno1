# Quicksort Pivots

in the lectures I only briefly mentioned strategies for determining a good pivot
for quicksort. The implementation on the slides simply picks the leftmost
element in the part of the array that we consider as a pivot. I also mentioned a
few other ways of picking a good pivot, e.g. randomly.

Median-of-three is also a good way of picking a pivot -- inspect the first,
middle, and last elements of the part of the array under consideration and
choose the median value. Using the probabilities for picking a pivot in a
particular part of the array (in the same way as we did on slide 34), argue
whether this method is more or less (or equally) likely to pick a good pivot
compared to simply choosing the first element. Assume that all permutations are
equally likely, i.e. the input array is ordered randomly.

Your answer must derive probabilities for choosing a good pivot and
quantitatively reason with them.

Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

Answer:
The Median-of-three method for selecting a pivot in Quicksort is more effective than simply choosing the leftmost element. This is because it increases the probability of selecting a good pivot. When using the leftmost element as the pivot, the probability of picking a "good" pivot, one that results in balanced partitions, is roughly 1/2,  since it’s equally likely to be anywhere in the array. In contrast, the Median-of-three method considers the first, middle, and last elements of the array. This method is more likely to select a pivot near the true median which improves the partition balance. The probability of picking a good pivot with the Median-of-three method is around 11/16. Which is significantly higher than the 1/2 probability of the leftmost element. Thus  the Median-of-three method reduces the likelihood of worst-case performance in Quicksort. While also leading to more balanced partitions and improved overall efficiency.

Sources:
Some lecture notes
ChatGPT to understand the probability when was incorrect

# Plagarism Statement
All exercises must contain the following statement: “I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”
