Download Link: https://assignmentchef.com/product/solved-csce314-homework-2-problem-set
<br>
<strong>Problem 1. </strong> Put your full name, UIN, and <em>acknowledgements of any help received </em>in the head comment in your .hs file for this assignment.

<strong>Problem 2. </strong> Chapter 4, Exercise 5. Using two nested conditional expressions in the definition is a requirement.

<strong>Problem 3. </strong> Chapter 4, Exercise 8.

<strong>Problem 4. </strong> Chapter 5, Exercise 6. Using a list comprehension and factors in the definition is a requirement. Include the definition of factors in your hw2.hs file (the definition is in the text as well as in my lecture slides).

<strong>Problem 5. </strong> Chapter 6, Exercise 5. Your answer should follow the style of examples such as reverse, (++), insert, and zip in pages 62–64 in the text. Write your answer neatly and clearly within a block comment {- ··· -}.

<strong>Problem 6. </strong> This problem has two subproblems. In Assignment 1, Problems 5 and 6, you implemented merge sort that sorts a list in an ascending order.

<ol>

 <li>Define a recursive function mergeBy that merges two sorted lists by the given criterion, for example, in an ascending order or in a descending order (so that the resulting list is also sorted). The type signature of mergeBy is as follows.</li>

</ol>

mergeBy :: (a -&gt; a -&gt; Bool) -&gt; [a] -&gt; [a] -&gt; [a]

Notice the difference from merge :: Ord a =&gt; [a] -&gt; [a] -&gt; [a] in Ch. 6 Exercise 7 such that mergeBy accepts three arguments, the first of which is a comparison function of type (a -&gt; a -&gt; Bool) that determines in which way the list is to be sorted. Such comparison function that returns a Boolean value (true or false) is called a <em>predicate</em>.

<ol start="2">

 <li>Using mergeBy that you wrote above and halve that you wrote for Problem 6 in Assignment 1, define a recursive function msortBy. The problem specification stays the same as that for <em>msort </em>in Ch. 6 Exercise 8, except the additional requirement of the first argument being a predicate. Thus, the type of msortBy is:</li>

</ol>

msortBy :: (a -&gt; a -&gt; Bool) -&gt; [a] -&gt; [a]

<strong>Problem 7. </strong>Chapter 7. Exercise 9.

<ol>

 <li> Define altMap.</li>

</ol>

altMap :: (a -&gt; b) -&gt; (a -&gt; b) -&gt; [a] -&gt; [b]

<ol start="2">

 <li> Explain how your altMap works when it is applied as below.</li>

</ol>

&gt; altMap (*2) (‘div‘ 2) [0..6]

<strong>Problem 8. </strong> Using map, filter, and (.) (function composition operator), define a function that examines a list of strings, keeping only those whose length is odd, converts them to upper case letters, and concatenates the results to produce a single string. concatenateAndUpcaseOddLengthStrings :: [String] -&gt; String

You need to import Data.Char in order to use the toUpper function (see the skeleton code).