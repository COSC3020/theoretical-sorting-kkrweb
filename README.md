# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.


//


Name: Kane Kriz

Last Edited: 19 March 2025
Feedback Request 1 Date: X


//


Response:

With access to only a black box implementation of the sorting algorithm as specified, you could attempt to verify this claim as follows:
You could begin by testing the functionality of the algorithm by generating a variety of input lists randomly.
You could then utilize the available black box implementation to sort each of these lists.
First ensuring that the sort is actually accurate, then measuring the time taken to sort each of input lists.
This would be done noting any irregularities or performance prefrences in regards to how the random generated input lists were made.

By comparing the time taken for the randomly generated input lists with the size of the input list, you could observe whether the algorithm's performance scales linearly with the input size. 
If true, the claim that the algorithm is truly O(n) would not be disproven yet. (though certainly not proven)

A next step would be to further test the algorithm and whether or not it maintains O(n) with more extreme edge cases and niche list possibilities.
Inputting lists with a variety of sizes, many (or little) occurrences of duplicate entries, empty lists, and lists with prevalance or lack of patterns in the lists could all be measured.

Considering whether the algorithm displays any unusual or unpredicted behavior in regards to these variables being modified could provide insight into the true functionality of the algorithm and how they may
be claiming that the algorithm is O(n). If the algorithm passed all of these edge cases and more specific list makeups without notable issue, you would move on to the below steps.

Comparison to known sorting algorithms and their proven complexities (unlike the doubtful O(n) from the problem) could prove immensely useful in gaining more information about the functionality of the algorithm.
You could consider any known sorting algorithm from class that we have covered and directly solved / been provided their asymptotic complexities.
You could then compare these known complexities with the claimed O(n) complexity of the secret algorithm.
Then testing if such comparisons are remotely reasonable through comparing the runtimes of the two algorithms against the same inputted list.

Theoretical argument portion - not complete yet

//

Plagiarism Acknowledgement: I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.


Citations:
