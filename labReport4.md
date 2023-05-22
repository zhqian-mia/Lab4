# Lab4  
For each numbered step starting right after the timer (so steps 4-9), take a screenshot, and write down exactly which keys you pressed to get to that step. For special characters like <enter> or <tab>, write them in angle brackets with code formatting. Then, summarize the commands you ran and what the effect of those keypresses were.


Below are the steps that we need to follow:  
* Log into ieng6
* Clone your fork of the repository from your Github account
* Run the tests, demonstrating that they fail
* Edit the code file ListExamples.java to fix the failing test (as a reminder, the error in the code is just that index1 is used instead of index2 in the final loop in merge)
* Run the tests, demonstrating that they now succeed
* Commit and push the resulting change to your Github account

**Step 4, log into ieng6 account.**
* Enter `cs15lsp23@ieng6.ucsd.edu<enter>`. Then, enter password and press `<enter>`. Now we login to ieng6 account successfully. 
![Image](https://github.com/zhqian-mia/Lab4/blob/main/ieng6%20login%20page.png?raw=true)  
  
**Step 5, now we want to clone the lab7 repository.** 
* Enter `git<space>clone<space>https://github.com/ucsd-cse15l-s23/lab7.git`. Now we have cloned the lab7 repo successfully.  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/git%20clone.png?raw=true)  
  
**Step 6, now let's run the test.sh file**
  * Enter `ls<enter>`, we are still outside of lab7. Enter `cd lab7<enter>`. Now, we are inside lab7 directory.
  ![Image}(https://github.com/zhqian-mia/Lab4/blob/main/store%20.png?raw=true)
  * Enter `bash<space>test<tab><enter>`, the terminal will automatically finish the command for us. The full command should be `bash<space>test.sh<enter>`. 
 ![Image](https://github.com/zhqian-mia/Lab4/blob/main/fail%20test.png?raw=true)  
  
**Step 7, the above image shows that our code did not pass the test file, thus we need to debug.**  
  
**Let's edit the code file ListExamples.java. Since we already know from the instruction that the bug is the index1 is used instead of index2 in the final loop in merge, things are much more easier.**
  * Enter `vim Lis<tab>.java<enter>`. Now we are able to edit the ListExamples.java file. The terminal now looks like this:  
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/after%20vim.png?raw=true)
  * Enter `kklllllllxi2<esc>`. In here, `k` stands for <up>, and `l` stands for <right>, `x` is used to delete the integer 1, `i` is used to initiate the Insert mode in vim, `2` allow me to enter integer 2 after the letter `x` of the word `index`. Finally, I pressed <esc> to exit the Insert mode in vim.
  * Enter `:wq<enter>`. In here, `w` stands for save and `q` stands for exit. 
  * Now, in the terminal, press the <up> button to repeat the last command `vim ListExamples.java`.  
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/before%20vim.png?raw=true)
**Now we can know that the modification are stored successfully.** 
  * Enter `:q!<enter>` to exit without storing changes.


kk l7 x i 2 esc
:wq enter
:q!
