# Lab Report 4 
Below are the steps that we need to follow:  
* Log into ieng6
* Clone your fork of the repository from your Github account
* Run the tests, demonstrating that they fail
* Edit the code file ListExamples.java to fix the failing test (as a reminder, the error in the code is just that index1 is used instead of index2 in the final loop in merge)
* Run the tests, demonstrating that they now succeed
* Commit and push the resulting change to your Github account

**Step 4, log into ieng6 account.**
* Enter `ssh<space>cs15lsp23@ieng6.ucsd.edu<enter>`. Then, enter `<password>` and press `<enter>`. Now we login to ieng6 account successfully. 
![Image](https://github.com/zhqian-mia/Lab4/blob/main/ieng6%20login%20page.png?raw=true)  
  
**Step 5, now we want to clone the lab7 repository.** 
* Enter `git<space>clone<space>https://github.com/ucsd-cse15l-s23/lab7.git<enter>`. Now we have cloned the lab7 repo successfully.  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/git%20clone.png?raw=true)  
  
**Step 6, now let's run the test.sh file**
  * Enter `ls<enter>`, we are still outside of lab7. Enter `cd lab7<enter>`. Now, we are inside lab7 directory.
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/store%20.png?raw=true)
  * Enter `bash<space>test<tab><enter>`, the terminal will automatically finish the command for us. The full command should be `bash<space>test.sh<enter>`. 
 ![Image](https://github.com/zhqian-mia/Lab4/blob/main/fail%20test.png?raw=true)  
  
**Step 7, the above image shows that our code did not pass the test file, thus we need to debug.**  
*Let's edit the code file ListExamples.java. Since we already know from the instruction that the bug is the index1 is used instead of index2 in the final loop in merge, things are much more easier.*
  * Enter `vim Lis<tab>.java<enter>`. Now we are able to edit the ListExamples.java file. The terminal now looks like this:  
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/after%20vim.png?raw=true)
  * Enter `kklllllllxi2<esc>`. In here, `k` stands for going up, and `l` stands for going right, `x` is used to delete the integer 1, `i` is used to initiate the Insert mode in vim, `2` allow me to enter integer 2 after the letter `x` of the word `index`. Finally, I pressed `<esc>` to exit the Insert mode in vim.
  * Enter `:wq<enter>`. In here, `w` stands for save and `q` stands for exit. 
  * Now, in the terminal, press the <up> button to repeat the last command `vim ListExamples.java`.  
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/before%20vim.png?raw=true)
**From the above image, we know that the modification are stored successfully.** 
  * Enter `:q!<enter>` to exit without storing changes.
    
**Step 8, now let's run the test.** 
  * Enter `bash<space>test.sh<enter>`. This command help us to run the test file. The terminal should look like this.
![Image](https://github.com/zhqian-mia/Lab4/blob/main/pass%20test.png?raw=true)  
    
*Therefore we know that the bug is fixed now and the ListExamples.java file pass all the tests.*  
    
**Step 9, now let's commit and push the resulting change to our Github account**
* Enter `git<space>add<space>.<enter>` to stage all the changes i made. 
* Enter `git<space>commit<space>-m<space>"lab7report"<enter>`. This allows us to commit the changes. The commit message I choose is `lab7report`. Now, the terminal now should look like this:
![Image](https://github.com/zhqian-mia/Lab4/blob/main/git%20add%20..png?raw=true)  
* Since we are still under the lab7 directory. Enter `pwd<enter>` in the terminal to get our current working directory, which is `/home/linux/ieng6/cs15lsp23/cs15lsp23se/lab7`.  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/push%20main.png?raw=true)
* Enter `git<space>push<space>/home/linux/ieng6/cs15lsp23/cs15lsp23se/lab7<space>main<enter>`. This command allows us to push the commit to our github using the push command. The branch name is `main`, and the orgin is `/home/linux/ieng6/cs15lsp23/cs15lsp23se/lab7`. The terminal now should look like this:  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/update.png?raw=true)
  
**Now, we have successfully finished all step 4 to step 9.**
