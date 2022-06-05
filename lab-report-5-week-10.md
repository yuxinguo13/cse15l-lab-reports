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

Actual output: `<foo(and(bar)>`

<img src = "image_report5/actual output 498.png">

Both my output and the provided repository output gave the wrong output as the output should actuallty be *[(foo)]*.


Part of my code that has error:


![image](https://user-images.githubusercontent.com/86458122/171515163-30fee906-8244-4ffe-8e2a-687c61101027.png)

Description of bug and how to fix it: I believe that the bug comes from the fact that I do not consider when there is an event where a code is in between more than one complete brackets. A condition of counting the brackets and checking the code between the brackets should be made to fix the error.

---

> ## Test file 2 : [499.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/499.md)

My output:

<img src = "image_report5/my output 499.png">

Repository output:

<img src = "image_report5/repository output 499.png">

Actual output: `foo\)\:`

<img src = "image_report5/actual output 499.png">

Both my output and the provided repository output gave the wrong output as the output should actuallty be an empty bracket *[]*, since there is no resulting link.


Part of my code that has error:


![image](https://user-images.githubusercontent.com/86458122/171516708-1673751b-b75c-43d5-badf-b3b493f05c6e.png)

Description of bug and how to fix it: I believe that the bug comes from this specific part of my code, before the if statement found on the picture above. I should have put a condition where if "!" is found in any index of the substring, the while loop should just break right away.


