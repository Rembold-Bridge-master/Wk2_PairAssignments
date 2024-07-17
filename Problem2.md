# Problem 1: Special Numbers


2520 is the smallest number that can be evenly divided by each of the numbers 1 through 10 (including 10!) without any remainder. Your goal today is to write a short program to determine how many numbers less than 1 million share this same trait. That is, how many numbers less than 1 million can be evenly divided by 1 through 10 without any remainder? I'll give you some milestones below that you can use to help you work through the problem.

1. Define a function called `number_of_special_numbers` which will take one argument: the max value of the range of integers you want to search over.
2. See if you can break the problem into a few separate pieces and write out what those pieces are as comments in your code.
3. Add code to solve each of the individual sub-problems you created. Sometimes solving these sub-problems as their own function is the best idea, but sometimes that might not make sense.
4. Bring all the sub-problem solutions together to get your final solution. Make sure you `return` this solution, don't just print it! I'm calling the function for you at the bottom of the script to print the results.

To give you some examples to test your code against, I will tell you that there are 3 numbers with this property less than 10,000, and 39 numbers with this property less than 100,000. The number of values with the described property actually follows a pretty interesting pattern if you keep increasing the maximum values by a factor of 10 each step!

