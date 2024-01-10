# Part One: Simplifying Expressions

1. O(n + 10) simplifies to O(n). We only keep the highest order term in big O notation because it will have the most impact on the running time for large values of n. Constants are also ignored.
2. O(100 \* n) simplifies to O(n). We ignore constants in big O notation because we're interested in how the running time grows with the size of the input.
3. O(25) simplifies to O(1). A constant expression denotes a constant time complexity, which is always O(1).
4. O(n^2 + n^3) simplifies to O(n^3). We only keep the highest order term.
5. O(n + n + n + n) simplifies to O(n). The sum of several n terms is still a linear function of n.
6. O(1000 \* log(n) + n) simplifies to O(n). The logarithmic term grows slower than the linear term, so the linear term dominates for large n.
7. O(1000 _ n _ log(n) + n) simplifies to O(n log n). The n log n term grows faster than the linear term.
8. O(2^n + n^2) simplifies to O(2^n). The exponential term grows much faster than the polynomial term, so it dominates.
9. O(5 + 3 + 1) simplifies to O(1). It's a constant time complexity.
10. O(n + n^(1/2) + n^2 + n \* log(n)^10) simplifies to O(n^2). Among all the terms, n^2 grows the fastest, so we keep it.

# Part Two: Calculating Time Complexity

1. logUpTo(n): The time complexity is O(n). The function contains a loop that runs n times, and the operations inside the loop (i.e., console.log(i)) are constant time.
2. logAtLeast10(n): The time complexity is O(n). Similar to the previous function, it runs a loop n times. The use of Math.max(n, 10) doesn't change the time complexity because it just ensures the loop runs at least 10 times.
3. logAtMost10(n): The time complexity is O(1). This is because the function will run at most 10 times due to the use of Math.min(n, 10), regardless of the size of n. Therefore, it's a constant time complexity.
4. onlyElementsAtEvenIndex(array): The time complexity is O(n), where n is the length of the array. The function runs a loop that iterates through each element of the array, so the time complexity is linear with the size of the input array.
5. subtotals(array): The time complexity is O(n^2), where n is the length of the array. This function contains a nested loop, where the inner loop runs up to i times for each i in the outer loop. This results in a quadratic time complexity.
6. vowelCount(str): The time complexity is O(n), where n is the length of the string. The function iterates through each
   character of the string once, so the time complexity is linear with the size of the input string. The operations inside the loop (i.e., checking if a character is in a fixed set of vowels and updating the count) are constant time.

# Part Three: Short Answer

1. True or false: n^2 + n is O(n^2). True. In big O notation, we only keep the highest order term because it will have the most impact on the running time for large values of n.
2. True or false: n^2 \* n is O(n^3). True. The multiplication of n^2 and n results in n^3, so the time complexity is indeed O(n^3).
3. True or false: n^2 + n is O(n). False. The term n^2 grows faster than n as n becomes large, so n^2 + n is not O(n), it's O(n^2).
4. What’s the time complexity of the .indexOf array method? O(n). In the worst-case scenario, .indexOf needs to iterate through the entire array.
5. What’s the time complexity of the .includes array method? O(n), similar to .indexOf, as .includes may need"Request to the upstream target timed out."
