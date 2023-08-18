## Algorithm
An algorithm is simply **a set of instructions for completing a specific task.**

Sometimes, it’s possible to have two different algorithms that accomplish the same task.

### Ordered Array
#### Insert
When inserting into an ordered array, we need to always conduct a search before the actual insertion to determine the correct spot for the insertion. This is one difference in performance between a classic array and an ordered array.

<img width="320" alt="Screenshot 2023-08-16 at 5 32 25 PM" src="https://github.com/viboloveyou12/Data-Structures-and-Algorithms-Note/assets/29854567/37c1b732-e864-4e57-b0c8-d249a55b07dc">

We can see in this example that there were initially four elements, and that insertion took six steps. In terms of N, we’d say that for N elements in an ordered array, the insertion took N + 2 steps in total. (search steps(3) + shift steps(2) + insert steps(1))

#### Search
When searching for a particular value within a **classic array**, we need to check each item until we find the value we're looking for. This process is referred to as **linear search**. 

With an **ordered array**, however, we can stop a search early even if the value isn’t contained within the array. Let’s say we’re searching for a 22 within an ordered array of `[3, 17, 75, 80, 202]`. We can stop the search as soon as we reach the 75, since it’s impossible for the 22 to be anywhere to the right of it.

Linear search can take fewer steps in an ordered array than in a classic array in certain situations. But classic arrays and ordered arrays don’t have tremendous differences in efficiency, or at least not in worst-case scenarios.

#### Binary Search
Binary Seach lets us keep on choosing the halfway mark in order to keep eliminating half of the remaining numbers.

> Note that binary search is only possible within an ordered array. With a classic array, values can be in any order, and we’d never know whether to look to the left or right of any given value. This is one of the advantages of ordered arrays: we have the option of binary search.

<img width="462" alt="Screenshot 2023-08-18 at 11 01 00 PM" src="https://github.com/viboloveyou12/Data-Structures-and-Algorithms-Note/assets/29854567/c1d54bfb-7163-4b87-900c-1843face0e2f">
