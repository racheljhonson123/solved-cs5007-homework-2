Download Link: https://assignmentchef.com/product/solved-cs5007-homework-2
<br>
<h1>1             Patterns</h1>

1) Write a function named rectangle that given two integers <em>n </em>and <em>m </em>prints out two identical rectangles of width <em>n </em>and height <em>m</em>, separated by an empty column, using the symbol ’∗’. You may use a loop or recursion. For instance, the call rectangle(4,6) should exactly lead to the following result on IDLE:

**** ****

**** ****

**** ****

**** ****

**** ****

**** ****

2) Write a function named triangle that, given a strictly positive integer <em>n </em>given as argument, prints out a triangle of height <em>n</em>, using the symbol ’∗’. You may use a loop or recursion.

By indexing the height from 0 (top) to <em>n </em>− 1 (bottom), this triangle should be such that: (1) Each row at depth <em>i</em>, <em>i &gt; </em>0, has two more stars than the number of stars of the previous row at depth <em>i</em>−1. (2) At depth 0, the function prints one star.

For instance, the call triangle(6) should exactly lead to the following result on IDLE:

∗

∗∗∗

∗∗∗∗∗

∗∗∗∗∗∗∗

∗∗∗∗∗∗∗∗∗

∗∗∗∗∗∗∗∗∗∗∗

<h1>2             Function on lists</h1>

Write a function clean1(aList) that takes a list of integers aList as argument, and returns a new list where multiple occurrences of values have been removed. <strong>The function should NOT modify its argument</strong>. This means that if we print the list (given as argument) after executing the function, it did not change. For instance, the following statements:

al = [1,2,3,4,4,4,5,1,2,1,5] newlist = clean1(al) print(al) print(newlist)

print the following result (a different order of values is acceptable):

[1,2,3,4,4,4,5,1,2,1,5]

[1,2,3,4,5]

<table>

 <tbody>

  <tr>

   <td> </td>

  </tr>

 </tbody>

</table>

<em>The principle of your algorithm may be the following:</em>

<ul>

 <li><em>Create a new empty list </em>tmp<em>.</em></li>

 <li><em>Use a “for loop” to fill </em>tmp <em>with each new value found in the argument list.</em></li>

 <li><em>Return </em>tmp<em>.</em></li>

</ul>

<h1>3             Function on lists</h1>

Write a function clean2(aList) that takes a list of integers aList as argument, and modifies this list, such as multiple occurrences of values have been removed. <strong>The procedure does not return a list: it modifies its argument (reference </strong>aList<strong>).</strong>

For instance, the following statements:

al = [1,2,3,4,4,4,5,1,2,1,5] print(al) clean2(al) print(al)

print the following result (a different order of values is acceptable):

[1,2,3,4,4,4,5,1,2,1,5]

[1,2,3,4,5]

<h1>4             Function on lists</h1>

Write a function named fct(aList) that takes a list of integers aList as argument and returns a string containing elements of the list that are a power of 2, all on the same line (i.e., without a new line after each printed value). Write a call to this function with argument [1<em>,</em>2<em>,</em>3<em>,</em>4<em>,</em>5<em>,</em>16<em>,</em>255<em>,</em>256<em>,</em>−1<em>,</em>−2<em>,</em>84], embedded in a print statement to see the result on IDLE.

<h1>5             Taylor Sinus</h1>

<strong>Required: To have points, you must use loop(s), NO recursion.</strong>

From calculus, we know that every continuously differentiable function can be represented as the sum of an infinite series. A finite subset of the series can be used to approximate the function. In this part, you will use Taylor series to approximate a sine function of an angle <em>x </em>in radians. Write a function taylor(x,n) that approximates the sin(<em>x</em>) by returning the sum of the first <em>n </em>elements of its Taylor series:

For instance, the following statements:

x = math.pi/2 print(math.sin(x)) print(taylor(x,7))

lead to the following result on the IDLE:

1.0

1.0000000006627803

<h1>6             Extra credit (5 points)</h1>

Implement a function consecutives(aList) that takes a list of integers as argument and return the maximum number of consecutive integers that are all equal, within this list. For instance, the following statements:

l1 = [1,1,1,3,3,4,4,4,4,4,3,1,7,3,3,4,4] l2 = []

l3 = [1,2,1,1,2,1,1] print(consecutives(l1)) print(consecutives(l2)) print(consecutives(l3))

lead to the following result on the IDLE:

5

0

2