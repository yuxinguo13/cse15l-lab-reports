# Lab Report2 Week4
[Other reports here](https://yuxinguo13.github.io/cse15l-lab-reports/)

### First Change
- Code change (deal with the blank line by checking the content of the next line)

<img src = "image_report2/change1code1.png" alt = "drawing" width = 650/>
<img src = "image_report2/change1code2.png" alt = "drawing" width = 600/>
<img src = "image_report2/change1test.png" alt = "drawing" width = 550/>

- Failure-including input: [test file 1](https://github.com/yuxinguo13/markdown-parser/commit/a53156ae21cbffd9f73410be4b36064613c3e6d0)

- Symptom of the code: it shows the infinitly loop and lack of heap space

<img src = "image_report2/symptom1.png" alt = "drawing" width = 500/>

- Relationship between the bug, the symptom, and the failure-inducing input
  - There is a empty line at the end of the test file
  - But in the code, we do not have method to deal with the blank line at the end of the file.
  - The empty line leads to the infinitely loop erroe in the test, and the not enough heap space, which lead to the failure of the test.

### Second Change

- Code change

<img src = "image_report2/change2code.png" alt = "drawing" width = 500/>

- Failure-including input: [test file 2](https://github.com/yuxinguo13/markdown-parser/blob/main/test-file3.md)

- Symptom of the code and test: the index of the arraylist is out of bound

<img src = "image_report2/change2test.png" alt = "drawing" width = 500/>

<img src = "image_report2/symptom2.png" alt = "drawing" width = 500/>

- Relationship between the bug, the symptom, and the failure-inducing input
  - In this test file, we don't have the () and only have the brackets.
  - Thus, our previous code which also detect the () would not work in this case.
  - When we trying to obtain the substring within the (), the index given would out of index.
  - Therefore, we change the code to only check the substring within the [].


### THird Cahange

- Code change

<img src = "image_report2/change3code.png" alt = "drawing" width = 500/>

- Failure-including input: [test-file-5](https://github.com/yuxinguo13/markdown-parser/blob/main/test-file5.md)

- Symptom of the code and test: the index of the arraylist is out of bound

<img src = "image_report2/change3test.png" alt = "drawing" width = 500/>

<img src = "image_report2/symptom3.png" alt = "drawing" width = 500/>

- Relationship between the bug, the symptom, and the failure-inducing input
  - The test file have link that both in the [] and ()
  - Our previous code would get the link that is in the () and would only obtain the link that is in the []
  - Thus, leading to the failure in test. That the actual output is less than the expected output
  - We could update the code to also find out the code with in the () to solve this problem.
  - 
