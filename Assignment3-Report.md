**SENG 637 - Dependability and Reliability of Software Systems**

**Lab. Report #3 – Code Coverage, Adequacy Criteria and Test Case Correlation**

| Group \#:              | 16  |
|------------------------|-----|
| Shahryar Soltanpour    |     |
| Mohammad Reza Kianifar |     |
| Muhammad Raihan        |     |

(Note that some labs require individual reports while others require one report
for each group. Please see each lab document for details.)

# Link of demo video

[Video Link](TODO://add-here-the-link-of-the-video)

It works for everyone with logged-in university account on outlook. Please [tell us](mailto:mohammadreza.kianifa@ucalgary.ca) if you had any problem.

# 1 Introduction

Text…

# 2 Manual data-flow coverage calculations for X and Y methods

Text…

# 3 A detailed description of the testing strategy for the new unit test

For reaching to more than 90% in line coverage, we wanted to do 2 things: 
1. Add new test cases for previous methods that didn't have 100% line coverage.
2. Add test cases for new methods to make them have 100% line coverage.

The approach is the same. We used the IntelliJ coverage tool that can show us the covered lines or branches within the 
number of hits they had. For each method, we saw the coverage hit map and then tried to add new test cases to cover all 
available lines. For conditions, we also tried to generate all possible cases of each term in that condition. The figure
bellow, shows an example of a previously covered method by black-box testing:

![Figure 1: An example of non-covered method](media/coverage-example.png)

We can see 3 types of color for each line:
1. <span style="color:green">Green</span>: Fully covered statement
2. <span style="color:red">Red</span>: Unreached statement
3. <span style="color:yellow">Yellow</span>: Partially covered condition. This happens when the condition has been true,
and only been passed.

So to make 100% line and branch coverage for this method, we added a new testCase with <i>lower > upper</i>.

By extracting the available branch for each method, and try to make the condition both true and false, we are able to go
for 100% line and branch coverage. We followed this technique to reach more than 90% of line coverage for both 
<i>Range</i> and <i>DataUtilities</i> classes.

# 4 A high level description of five selected test cases you have designed using coverage information, and how they have increased code coverage

We have added some new test cases for Range and DateUtilities class to increase our line, method and branch coverage. There were 4 out of 9 methods in DateUtilities class that were not tested in the previous assignment. One of them is the 'equal' method that checks if two given double[] arguments are equal or not. Here is a description of test cases written for this method:
![img_1.png](media/equal_testcases.png)
# 5 A detailed report of the coverage achieved of each class and method (a screen shot from the code cover results in green and red color would suffice)

Text…

# 6 Pros and Cons of coverage tools used and Metrics you report

Text…

# 7 A comparison on the advantages and disadvantages of requirements-based test generation and coverage-based test generation.

Text…

# 8 A discussion on how the team work/effort was divided and managed

Text…

# 9 Any difficulties encountered, challenges overcome, and lessons learned from performing the lab

Text…

# 10 Comments/feedback on the lab itself

Text…
