# Lab Report 4
## Khoi Nguyen
### Introduction
For the lab report this week, I will be performing the tasks listed below. For each numbered step starting right after the timer (so steps 4-9), I will be detailing exactly which keys I pressed to get to that step. Furthermore, explaining the commands I ran and what the effect of those keypresses were. <br>
**NOTE**: The commands and steps that I am detailing in this report will mostly be focused on steps that are starting after the timer as explained above. This includes step 4 to 9. <br>

### Explanation of Steps
1. **Setup**: Delete any existing forks of the repository you have on your account
2. **Setup**: Fork the repository
3. **The real deal**: Start the timer!

4. Log into ieng6 <br>
![image](lab4_1.jpg)<br>
<u> Commands </u> <br>
Username: `<up>` <br>
Password: `<CTRL>` + `<C>` (copied passwords from Note's app) -> `<CTRL>` + `<V>` + `<enter>` <br>
<u> Explanation </u> <br>
- Since I have previously typed in the `ssh` command, the command has already been stored in my bash history. Hence I was able to quickly type the `<up>` arrow to quickly access the command in my history.
- My account password is stored in my Note's app. Hence I was able to quickly copy (`<CTRL>` + `<C>`) and paste (`<CTRL>` + `<V>`) my password to login.

5. Clone your fork of the repository from your Github account <br>
![image](lab4_2.1.jpg)<br>
![image](lab4_2.2.jpg)<br>
<u> Commands </u> <br>
`<CTRL>` + `<C>` (link of github lab7) -> `git clone` +  `<CTRL>` + `<V>` + `<enter>` <br>
<u> Explanation </u> <br>
- First I went to the course website to copy (`<CTRL>` + `<C>`) the link of the repository. A GitHub repository is where your project files are stored. When you clone your repository, you’re simply making a copy of the repository from GitHub and saving it to your machine. The `git clone` command copies an existing Git repository. Hence `git clone https://github.com/ucsd-cse15l-s23/lab7` clone the repository which has a subset of the code from the week 3 lab. 

6. Run the tests, demonstrating that they fail <br>
![image](lab4_3.jpg)<br>
<u> Commands </u> <br>
`cd` + `lab7` + `bash`+ "t" + `<tab>` + `<enter>` <br>
<u> Explanation </u> <br>
- First we need to make sure we are in the correct directory. The target directory is `lab7`. To change the working directory, I used the `cd` command.
- The `bash test.sh` command is used to execute a Bash shell script named `test.sh`. A shell script is a file containing a series of commands that are interpreted and executed by the Bash shell. This command will help us test whether `ListExamples.java` file is successful. I first typed the letter "t" to indicate the bash shell script name starts with a letter `<t>`. Since there is only one bash shell script name starts with a letter `<t>` in the working directory, the `<tab>` shortcut will auto-complete.
- In the picture above, we can clearly see since the apporiate changes were not made, the test fails.

7. Edit the code file to fix the failing test <br>
![image](lab4_6.4.jpg)<br>
*Figure 7.1* <br>
![image](lab4_6.1.jpg)<br>
*Figure 7.2* <br>
![image](lab4_6.2.jpg)<br>
*Figure 7.3* <br>
![image](lab4_6.3.jpg)<br>
*Figure 7.4* <br>
<u> Commands </u> <br>
Figure 7.1: `vim`+ "L" + `<tab>` + "." + `<tab>` + `<enter>` <br>
Figure 7.2: `/<change>` + `<enter>` (cursor should be on c) -> searches for the line with the given method that needs to be edited <br>
Figure 7.3: `<j>` + `<l>`+ `<l>`(cursor should be on 1) + `<x>` <br>
Figure 7.4: `<i>` + `<2>` + `<escape>` + `:wq` + `<enter>` <br>
<u> Explanation </u> <br>
- Figure 7.1: When you run the command `vim` in a terminal, it launches the Vim editor. I typed the letter "L" to indicate I am looking for a file that starts with said letter. There are two files in the repository: "ListExamples.java" and "ListExamplesTest.java". I was able to ultilize the `<tab>` shortcut to ato-complete my search. Then typing "." and `<tab>` to auto-complete my search for a ".java" file. 
- Figure 7.2: The `/` command searches forward a specific term. In this case I am looking for the word "change" which will take me to the line just above our desired code to fix. 
- Figure 7.3: The `<j>` command will move our cursor down while the `<l>` command will move our cursor in the right direction. We will go down one line then right 2 spaces until the cursor is on the number 1. The `<x>` command will then remove the character at the current position of the cursor. Since the cursor position is at 1, calling the `<x>` command will remove the character `<1>`.
- Figure 7.4: When calling the `<i>` command, we are entered into insert mode at the current cursor position. We then enter the character `<2>` to insert the character at the given cursor position. It is important to note that we will remain in insert mode until we use `<escape>` to exit. The `<:w>` command saves the file while the `<:q>` command exits out of Vim. We can use both the command at once (`:wq` + `<enter>`), to quickyly both save the changes then quit Vim.

8. Run the tests, demonstrating that they now succeed <br>
![image](lab4_4.jpg) <br> 
<u> Commands </u> <br>
`<up arrow>` + `<up arrow>` <br>
<u> Explanation </u> <br>
- Since I have previously called the `<bash test.sh>` command, it is not saved in my bash history. Out of conveniece, I was able to press the `<up>` arrow twice to retrieve my command.

9. Commit and push the resulting change to your Github account <br>
![image](lab4_5.jpg) <br> 
<u> Commands </u> <br>
`<git commit -am “lab4”>` + `<git push>` + `<username>` + `<github password>` <br>
<u> Explanation </u> <br>
- The `<git commit -am “lab4”>` command in Git is used to create a new commit with a commit message, including changes to tracked files. I used the `<git commit>` to create a new commit. Then `<-a>` command to automatically stage (add to the index) all tracked files that have been modified or deleted. The `<m>` is to add a meaningful commit message. In my case, my commit message was just `<lab4>`.
- I then utilized the `<git push>` command to push your local Git repository to a GitHub repository. I had to authenticate with GitHub hence entering my GitHub username and password. 
<br>
**NOTE**: I have been having issues with authenticating my GitHub as well as generating SSH Keys for ieng6/Github. I have asked for help during lab sessions but my IA was unable to identity the issue. I have been recommended to go to office hours with Joe to seek possible solutions to this issue which is held after the due date of this lab report. At the time of this submission, the authentication will appear as denied but I am working on getting this fixed. Thank you! <br>
