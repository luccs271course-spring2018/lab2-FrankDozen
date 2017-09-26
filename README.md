# COMP 271 F17 002 Lab 2

# Team project

Work in teams of two

# Objectives

An understanding of the following concepts and techniques:

- entity objects
- linear search
- binary search
- algorithmic complexity
- arrays versus lists
- [optional values](https://docs.oracle.com/javase/8/docs/api/java/util/Optional.html)
- DRY and factoring out methods
- final-correctness
- automated unit testing using JUnit
- testing for exceptions
- test fixtures and assertions

# Instructions

1. Review the code.
2. Run the code for various inputs to gain an understanding of what it does.
3. Complete the items marked TODO in the code and get the tests to pass.
4. Create a markdown document called Answers.md and answer the questions in the next section.

# Questions

- What is the complexity of each of the four search methods in terms of array or list size n?
For findTeamMinFunding and findTeamPosition each operations is ran once for each item on the list, value of n. However, findTeamMinFundingFast cuts the search space in half, thus it's complexity is in porpotion to how many divisions it takes to narrow the search space (O(log(n))).

- What happens in the case of binary search if the array is not sorted?
    There will be a logic error. The program may do a number of glitches such as an endless loop.

- What is the purpose of constructor argument validity checking?
    It prevents runtime errors caused by methods attempting operations on null values.

- What is the purpose of using the keyword `final` with variables and arguments?
    The key word 'final' initializes variables and arguments so that their values can not be altered.

- What are alternatives to using `Optional` and how do they compare?
    You can use @Nullable and @NonNull which are more efficent, however, it is only supported in a few IDES.
