# ugly-numbers

This JavaScript code is intended to solve a rather artificial problem, which is difficult to talk about without defining some local terminology:
1) The term "ugly number" as used here refers to any number divisible by at least one of the following numbers: 2, 3, 5, 7.
2) Given some finite series of digits <i>S</i>, I'll use the term "substring-derived expressions" to refer to the set of mathematical expressions that can be derived by inserting +, -, or nothing between each of <i>S</i>'s digits [independently]. For conciseness, I will sometimes refer to this set as .SDE(<i>S</i>). Thus, for instance, if <i>S</i> = "123", SDE(<i>S</i>) = <i>S</i>'s substring-derived expressions = {123, 12+3, 12-3, 1+23, 1+2+3, 1+2-3, 1-23, 1-2+3, 1-2-3}. More generally, taking <i>n</i> to be the number of digits in <i>S</i>, S's substring-derived expressions number 3<sup>(n-1)</sup>.

Using the above terminology, the problem to be solved is: given <i>S</i>, find the subset of SDE(<i>S</i>) containing all and only those elements of SDE(<i>S</i>) that evaluate [when interpreted as arithmetic expressions using the standard + and - operators on numbers written in base-10] to ugly numbers.
