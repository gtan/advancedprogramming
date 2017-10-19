# Lesson 6: More Practice

**To start this lesson, students should**:

**By completing this lesson, students will**: 

Becoming a good coder is all about practice. This lesson will go through a couple practice problems to help you solidify what you've learned already.
 
## Has 22

The first question actually is on another website. Go [here](http://codingbat.com/prob/p119308) for the first question, then return and we can continue.

## Max Ascending Sublist Size

Now, you can go ahead and download exercises.py. Find this function:

	#returns the size of the maximum increasing sublist in the list of numbers supplied in the variable, nums
	def max_ascending_sublist_size(nums):
		#TODO: implement this!
		return -1
		
For this problem, we will a function that takes an list of integers and returns the size of the largest ascending sublist. An ascending sublist is one where each element is greater than the previous number in the list. For example, for the list `[1, 5, 9, 9, 8, 7]`, `[1, 5, 9]` is an ascending sublist, but `[9, 9]` (not strictly greater), `[9, 8, 7]` (descending), and `[1, 5, 8]` (not consecutive) are not. 

	max_ascending([5, 10, 15, 20]) --> 4
	max_ascending([1, 3, 2, 4, 5, 6, 1]) --> 3
	max_ascending([4, 3, 2, 1]) --> 1
	
### Big O Practice

Here's a challenge now. Once you're satisfied with your solution to this question, *what is the Big O runtime?* Once you think you have an answer, check with a mentor to see if you're right.

## Chocolate

Next question is also on codingbat! Go [here](http://codingbat.com/prob/p190859) for the next question, then come on back and we can continue.

### Big O

Once you've finished that one, what do you think the Big O runtime is? 

> **Hint:** If you came up with an O(N) solution, there might actually be another one that is O(1), meaning it will take the same amount of work no matter how big the input is. You don't need to spend a long time trying to figure out the O(1) solution if so, but in general, this is always the best runtime!
 
## Translation

The next exercise is in this function:

	#reads in the translation between orig and translated, and returns the result of that same translation on words
	def translate(orig, translated, words):
		#TODO implement this!
		return words
		
For this function, we are going to write a function that looks at two strings, `orig` and `translated`, then applies the same translation to `words` and returns the result.

In this translation, we can assume that the rule is that every letter in `orig` will be substituted a single letter, and that that letter will always be the same. Therefore, you can assume that `translated` will always be the same length as `orig` and that every letter at the same index in the two strings should always be swapped in your resulting translation.

Letters that don't appear in `orig` should remain the same

For example:

	translate("abc", "bca", "ababccce") -> "bcbcaaae"
	translate("abcdefg", ".pppppp", "ahwbccdz") -> ".hwppppz"
	translate("q", "p", "qpeo") -> "ppeo"
	
**Again, see if you can figure out the Big O runtime after you finish this.**