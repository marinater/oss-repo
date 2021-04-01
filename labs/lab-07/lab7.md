Samarth Patel

# Lab 7

## Checkpoint 1: Getting started

![image-20210331160903660](./img1.png)

![image-20210331161056608](./img2.png)

## Checkpoint 2: Executing the tests

### Part 1

- The cdash link provided links to a dashboard that has one row for each build. Builds that have failed tests have the 'Fail' column of the table highlighted in red with a nonzero entry indicating how many tests failed. You can click on this text (it's a hyperlink) and it will take you to another page that displays the exact test cases that failed. Example of one of these pages can be found [here](https://open.cdash.org/viewTest.php?onlyfailed&buildid=7133522)
- The link I included above has 3 failures. You can see the overall error condition by looking in the 'Details' column. One of them says timeout, which could be indicative of a process hanging for some reason. More details can be found by clicking the name of tests in the 'Name' column (they are hyperlinks). This will take you to a page of the actual test output, which can more easily help debug what went wrong without having to run the test locally. Doing this, I found that one of the tests (found [here](https://open.cdash.org/test/375121710)) is failing because a cmake file has incorrect syntax.
- I found a `macOS-make` build that has 1 failing test (found [here](https://open.cdash.org/test/374952993?graph=Processors)). The error is that one test is NOT timing out when it is expected that it does. This does not overly concern me, but someone with more familiarity contributing to CMake would have better knowledge of how critical this test is. Otherwise, the mac builds are fairly green across the board.

### Part 3

There are no errors in the build.

### Part 4

[Link to submission](https://open.cdash.org/build/7134756)

![image-20210331201555084](./img3.png)

## Checkpoint 3

![image-20210331204226183](./img4.png)

![image-20210331205038504](./img5.png)

The fix was to simply change the copyright year from 2000-2020 to 2000-2021

![image-20210331205806612](/Users/marinater/Library/Application Support/typora-user-images/image-20210331205806612.png)

After this change, the tests ran successfully

![image-20210331205533950](./img6.png)

### Checkpoint 4

Repo (with updated readme): https://github.com/marinater/Step5

![image-20210331221841624](./img7.png)

![image-20210331221908085](./img8.png)

After adding a test

![image-20210331222153409](./img9.png)

![image-20210331222615524](./img10.png)

![image-20210331222642440](./img11.png)

## Checkpoint 5

![image-20210331222912650](./img12.png)

