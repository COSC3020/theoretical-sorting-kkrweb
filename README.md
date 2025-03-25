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

Start Date: 23 March 2025

Last Edited: 24 March 2025

Feedback Request 1 Date: 24 March 2025


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



Theoretical argument:
The claim that the created sorting algorithm has a sorting time of O(n) given the context in the problem description could not possibly be theoretically correct. 
This is due to first informally considering known comparison based sorting algorithms (without extra conditions / information potentially associated with them to alter their necessary implementation, but then they potentially wouldnt be comparison based) 
...having at best a worst case complexity of O(nlogn) across all algorithms meeting the conditions of a standard comparison based algorithm.

This demonstrates how truly revolutionary such an alogorithm would be, if even possible, making such an algorithms actual creation that much more farfetched.
I suppose bringing that up isn't exactly theoretical, but I will keep it in because it is just another layer of reasoning to this being unlikely.

Formally, a O(n) complexity would further not be possible because of the number of permutations that inherently exist from a list.
Consider a list of size n. The number of permutations of a list of size n is n!.
As we are considering the worst case (and I suppose the general functionality / complexity of the algorithm), all n! possible permutations.
Covering all n! possible permutations in a guaranteed at worst complexity of O(n) is impossible, as the number of elements scaling with O(n) linearly versus the scaling of n! compares in the worst case do not allign.
The best case for a worst-case outcome of a standard sorting algorithm (covering all n! permutations) is at best O(nlog(n)), visible when considering the worst case complexities of heap and merge sort, as examples.

Any algorithm that magically could be able to reach a true worst case O(n) complexity would thus have to not truly be a two-element comparison algorithm in truth, as it violates this established best case of worst cases.
As we know, a best case of O(n) for a sorting algorithm is a simple reality that can occur depending on something such as a sorted list being provided to a particular algorithm (provided such an algorithm responds well to an already sorted list). 
However, the moment an algorithm begins to claim for a trraditional comparison based algorithm that O(n) is guaranteed, that is where problems arise, as explained above.



//

Plagiarism Acknowledgement: I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.


Citations:
“Software Engineering | Black Box Testing - GeeksforGeeks.” GeeksforGeeks, 25 May 2018, www.geeksforgeeks.org/software-engineering-black-box-testing/.
“Time Complexities of All Sorting Algorithms.” GeeksforGeeks, 10 Jan. 2023, www.geeksforgeeks.org/time-complexities-of-all-sorting-algorithms/.
