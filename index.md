# Lab Report 4
## Khoi Nguyen
### Introduction
For the lab report this week, I will be performing the tasks listed below. For each numbered step starting right after the timer (so steps 4-9), I will be detailing exactly which keys I pressed to get to that step. Furthermore, explaining the commands I ran and what the effect of those keypresses were. <br>
**NOTE**: The commands and steps that I am detailing in this report will mostly be focused on steps that are starting after the timer as explained above. This includes step 4 to 9. <br>

### Explanation of Steps
1. **Setup**: Delete any existing forks of the repository you have on your account
2. **Setup**: Fork the repository
3. **The real deal**: Start the timer!

4. Log into ieng6
![image](lab4_1.pdf)<br>
<u> List of Commands </u> <br>
Username: `<up>` <br>
Password: `<CTRL>` + `<C>` (copied passwords from Note's app) -> `<CTRL>` + `<V>` <br>
<u> Explanation </u> <br>
- Since I have previously typed in the `ssh` command, the command has already been stored in my bash history. Hence I was able to quickly type the `<up>` arrow to quickly access the command.
- 
5. Clone your fork of the repository from your Github account
CNTRL + C <link of github lab7> -> git clone +  CNTRL + V
  
6. Run the tests, demonstrating that they fail
Cd lab7
bash test.sh (should fail with og code)
bash<tab>

7. Edit the code file to fix the failing test
vim ListExamples.java -> opens the code to List.Examples.java
vim <tab> +.java
/change<enter> (cursor should be on c) -> searches for the line with the given method that needs to be edited
j l l  x (cursor should be on 1) 
i<2> <escape> :wq <enter>
  
8. Run the tests, demonstrating that they now succeed
bash test.sh (should be good)
Up arrow, up arrow

9. Commit and push the resulting change to your Github account
<git commit -am “name”>
git push
Enter username
Enter github password


