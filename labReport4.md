# Lab Report 4 
Below are the steps that we need to follow:  
* Log into ieng6
* Clone your fork of the repository from your Github account
* Run the tests, demonstrating that they fail
* Edit the code file ListExamples.java to fix the failing test (as a reminder, the error in the code is just that index1 is used instead of index2 in the final loop in merge)
* Run the tests, demonstrating that they now succeed
* Commit and push the resulting change to your Github account  

***  

**Step 4, log into ieng6 account.**
* Enter `ssh<space>cs15lsp23@ieng6.ucsd.edu<enter>`. Then, enter `<password>` and press `<enter>`. Now we login to ieng6 account successfully. 
![Image](https://github.com/zhqian-mia/Lab4/blob/main/real%20login.png?raw=true) 

***  

**Step 5, now we want to clone the lab7 repository.**   
*Since I already generate the ssh key for github, i can git clone the ssh link of lab7.*
* Enter `git<space>clone<space>git@github.com:zhqian-mia/lab7.git<enter>`. Now we have cloned the lab7 repo successfully.  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/real%20git%20clone.png?raw=true)  

***  

**Step 6, now let's run the test.sh file**  
  * Since we are still outside of lab7. Enter `cd lab7<enter>`. Now, we are inside lab7 directory.
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/cd%20lab7.png?raw=true)
  * Enter `bash<space>test<tab><enter>`, the terminal will automatically finish the command for us. The full command should be `bash<space>test.sh<enter>`. 
 ![Image](https://github.com/zhqian-mia/Lab4/blob/main/bash%20fail.png?raw=true) 
 
***   

**Step 7, the above image shows that our code did not pass the test file, thus we need to debug.**    
*Let's edit the code file ListExamples.java. Since we already know from the instruction that the bug is the index1 is used instead of index2 in the final loop in merge, things are much more easier.*
  * Enter `vim Lis<tab>.java<enter>`. Now we are able to edit the ListExamples.java file. The terminal now looks like this:  
  ![Image](https://github.com/zhqian-mia/Lab4/blob/main/before%20change%20vim.png?raw=true)
  * Enter `kklllllllxi2<esc>`. In here, `k` stands for going up, and `l` stands for going right, `x` is used to delete the integer 1, `i` is used to initiate the Insert mode in vim, `2` allow me to enter integer 2 after the letter `x` of the word `index`. Finally, I pressed `<esc>` to exit the Insert mode in vim.
  * Enter `:wq<enter>`. In here, `w` stands for save and `q` stands for exit.
  * Now, in the terminal, press the <up> button to repeat the last command `vim ListExamples.java`.  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/vim%20after%20change.png?raw=true)  
   
*From the above image, we know that the modification are stored successfully.* 
  * Enter `:q!<enter>` to exit without storing changes. 
 
***  
 
**Step 8, now let's run the test.**  
  * Enter `bash<space>test.sh<enter>`. This command help us to run the test file. The terminal should look like this.
![Image](https://github.com/zhqian-mia/Lab4/blob/main/bash%20pass.png?raw=true)    
*Therefore we know that the bug is fixed now and the ListExamples.java file pass all the tests.*  
 
***  
   
**Step 9, now let's commit and push the resulting change to our Github account.**  
* Since we are still in the directory of lab7, enter `git<space>status<enter>`. This command will allow us to see the current git status in the linux system. Thus we can see the the file ListExamples.java has been modified. Follow the instruction in the terminal to commit the change.
* Enter `git<space>add<space>.<enter>`. This command is used in Git to stage all changes in the current directory and its subdirectories for the next commit.
* Enter `ls<enter>`. I did this to check if I am still in the lab7 directory.
* Enter `git<space>status<enter>`. Now from the terminal we can know that the modification has been commited successfully.  
*Below is a screenshot of the above three steps*
![Image](https://github.com/zhqian-mia/Lab4/blob/main/git%20status.png?raw=true)  
* Enter `git<space>commit<space>-m"glass"<enter>`. This command allows us to commit the edit and name it with a message of your choice. I choose the word "glass".  
* Enter `ls<enter>` to check if i am still inside the lab 7 directory. (This step is redundant, not really need to use it).  
* Enter `git<space>status<enter>`. This command allow us to get a glance on the current status of git on our remote server. Right now from the terminal we can see that the changes we made previously have been commited successfully.  
![Image](https://github.com/zhqian-mia/Lab4/blob/main/ss2.png?raw=true)
* Follow the instruction, we enter `git<space>push<enter>`. This command allow us to upload or send our local commits to the main. Now the terminal looks like this:
![Image](https://github.com/zhqian-mia/Lab4/blob/main/git%20push%20successfully.png?raw=true)
*Now we know that the changes are successfully commit and push to the main to my github account. To double check, this is what it looks like on the github website.*   
![Image](https://github.com/zhqian-mia/Lab4/blob/main/ccc.png?raw=true)
*It shows that the ListExamples.java was edited not long ago.*  
   
***  
   
**Now, we have successfully finished all step 4 to step 9.**
