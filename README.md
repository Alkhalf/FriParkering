# FriParking
TestNew2,FriParking App är en gratis app som visar alla platser med fri parkering i hela Sverige. Appen är gratis att använda och det är också gratis att skapa ett konto


fadshi



# Git Strategy

## How we will work
We will work in a **issue** based Continuous integration, aka CI, every task and ideas will be created with an issue where you have task inside of them. If the task is complicated or is different but is depended on the task you are working on, you can create a sub task which will be getting their own issue-number which you can create the new branch for. And when you have finished working on that sub-task you create a **pull-request** to your previous task (parent-task).

### Good to know
Master branch (or main branch) will not be touched by any developer directly. If you want to change something you will need to create a new branch which you create a pull-request to main-branch

## How to create branches
You will create git branch with a specific structure that is based on the Git issue number.  
When creating your new branch:  
1. Make sure you have marked as *assign* the specific issue you want to work with.
2. When creating a branch make sure to have in mind that you will create a branch only for a specific task and not more. If there is a lot more sub-task create sub-issue for that task.
3. Now that you have understood the principle, now is the time to create your branch. You will create a branch that looks like this.
```
MurtadhaAlobaidi/issue/11
```
- *MurtadhaAlobaidi*, Is the github username.
- *issue*, is where the task located.
- *11*, is the issue number.

**So the template of this git branch is**:
```
<username>/issue/<issue-number>
```

## How to commit
When committing your work make sure that you do not select everything and commit instead **choose** what to commit. For example:
```
/* This are the files you have changed */
1. README.md // only added space at the end of the file.
2. views/login.ejs // Added a component.
3. functions/views/home.ejs // Created a new component.
```

Most of the time is correct to have time together but in this case where we are learning try and separate them from each commits. The first commit can be:
```
#11: feat: Created a new views
```
And the second one can be:
```
#11: add: Added a home to views
```
And here you can see a structure.
- *#11*, is the issue number.
- *feat*/*add*/*fix*/*rm*, are different categories of your commits.
  - *feat*, is used when you are creating something new.
  - *add*, is used when you are adding a new code/text into a existing file.
  - *fix*, is used when you are fixing a existing code.
  - *rm*, is used when you are removing a code block or file.
- *Text*, after the the categories added in the beginning of the commit you will add the text. *Keep it short and informative on what you have done.*

**So the template of this git branch is**:
```
#<issue-number>: <categories>: <Text>
```
