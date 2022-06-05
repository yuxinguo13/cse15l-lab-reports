# Lab Report5 Week10

[Other reports here](https://yuxinguo13.github.io/cse15l-lab-reports/)

I found the test with different results by adding `echo $file` in script.sh. to print the name of test files before its output.
Then I check through the output and find these two files.

<img src = "image_report5/output for two files.png" width = 300>

There are the links to the two files

_File 498_
- [link to first text file](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/498.md)

_File 499_
- [link to second text file](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/499.md)

---
> ## Test file 1 : [498.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/498.md)

My output:

<img src = "image_report5/my output 498.png">

Repository output:

<img src = "image_report5/repository output 498.png">

Actual output: 

<img src = "image_report5/actual output 498.png">

Both my output and the output from the provided repository are inconsistent with the correct output as the output should be `<foo(and(bar)>`

Error in my code:

<img src = "image_report5/error my code 498.png">

Description of bug and how to fix it: I found that after find the index of the (, I find the ) that is after this sign. That's why my output only get the 
`<foo(and(bar` and doesn't have the `)>`. So in order to fix the bug, I believe that I need to find the ) from the end of the text rather than the ) that is immediately after the ( brucket.

Error in provided repository:

<img src = "image_report5/error in provided code 498.png">

Description of bug and how to fix it: In the findCloseParen method I find that the method assume that the findCloseParen is at one index after the open paren. This is wrong. So, to fix the bug, we could use the indexof to find the close paren first. 

---

> ## Test file 2 : [499.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/499.md)

My output:

<img src = "image_report5/my output 499.png">

Repository output:

<img src = "image_report5/repository output 499.png">

Actual output: 

<img src = "image_report5/actual output 499.png">

Both my output and the output from the provided repository are inconsistent with the correct output as the output should be `foo\)\:`

Error in my code:

<img src = "image_report5/error my code 499.png">

Description of bug and how to fix it: For this text, my code doesn't consider that pairing of paren. For a ( would be a ), it's hard to tell the pairing of brucket. I think I could fix the bug by using stack to store the existing paren, so I could get rid of this bug.

Error in provided repository:

<img src = "image_report5/error in provided code 499.png">

Description of bug and how to fix it: This is similar to my previous bug, after finding the (, the code finds the ) immediately. This is inccorect since my might need to find the ) from the back of the text rather than from the index of (. 
