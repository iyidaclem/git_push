# Automating Your Git Commands
This is a mini project on automating the most frequently used git commands 
- git add 
- git commit and 
- git push

# Files
# [git_push.sh](git_push.sh)

I was opportune to get admitted into ALX Software engineering scholarship in August 2022 (Cohort 9) to be precise. We covered a lot of software engineering foundational courses like Linux command line, bash scripting, version control systems and lots more. Basically the program is practical based and every task has to be pushed to GitHub repository so that their checker can pass it.
This is the kind of program any aspiring software engineering wouldn't like to miss. The daily tasks are really technical and has an incremental effect based on the objective of the project being tackled. One of the things I found boring about the tasks is the fact that you will need to push the code for every single task to GitHub so that the checker can actually verify whether the code is correct or not.
For every single task you are going to do the following: 
- Git add .
- Git commit -m "Message here"
- Git Push

Now imagine if you have 20 tasks in one project that means you are going type the above commands 20 times.
20 * 3 = 60;
That means you are going to type 60 git command for you to complete the project of the day.
 That figure is actually minimum number of git commands you will type assuming you did not make any mistake at all which is not possible. But if you eventually make any mistake, then it means you are going to repeat it.
As people usually says that programmers are lazy (lols) that led me to find a way of automating these commands.
So I decided to create a bash script to automatically perform 
- git add
- git commit and 
- git push

## STEP 1: CREATE THE SCRIPT 
Create the script file using your favorite editor, in my case I use vim. Add the these lines of code inside it
My file name  [git_push.sh](git_push.sh)
Now save the file.

## STEP TWO: MAKE THE FILE EXECUTABLE
Make the script which you just created to be executable by typing the following code in your terminal and press enter
chmod + x git_push.sh
Make your bash script executableSTEP THREE: ADD THE FILE TO YOUR PATH
Now move the file into your path. This is to a kind of give it a global scope.
`mv git_push.sh  /bin/`
You may also add sudo to your command if you encounter permission error.
sudo mv git_automation /bin/
Note: Using sudo will prompt for you password, then enter you password and press enter

## STEP FOUR: TEST YOUR SCRIPT
Run you script by just typing :
`git_push.sh "commit message"`

Press enter and boom you have committed and push your project to Github.

'Congrats'!!! You have successfully done: "git add ., git commit and git push" in one line of code
You can learn bash scripting from http://linuxcommand.org/
You can get the source code of this script from 
Thanks for reading!!!
