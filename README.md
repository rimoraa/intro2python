# Week 2 -- Intro to Python Part 1: HW1

## Class 1 catch-up - fixing Git and getting Jupyter Notebooks to work
Apologies again for things not working in class. The first thing we need to do is set up our intropython folder through git such that we can push, or upload, our scripts and files to the remote repository we previously set up online. We had an issue in class because we used https instead of ssh to set up our git repo locally, on our computer. If you're curious about how these server protocols work, feel free to come chat with us before class, but for now this is outside the scope of the class.

To set up our folder to work with SSH, we just need to enter a few commands. Please navigate to your intro2python repository folder by opening the terminal and entering the following commands:
```
cd documents
```
and
```
cd intro2python
```
To confirm that you're in your new directory, type in:
```
git status
```
If you receive an error, check that you're in the directory we created during class. If this does not solve the issue, email us so we can troubleshoot. Next, we  will swap over the repository to SSH verification by typing in the following command. All this command does is swap where git tries to upload the files, such that it sends them to an internet address that expects SSH credentials. Make sure to swap <USERNAME> for your username (drop the brackets):
```
git remote set-url origin git@github.com:<USERNAME>/intro2python.git
```
Now try to upload your files/push them to the online repoistory via:
```
git push
```
If no error is thrown, you should be set! If you get an error, please email us. You can verify that everything worked by navigating to your repo online and checking to see if you see your files online. 
#### DELIVERABLE 1: Please submit a screenshot of your repo online to the courseworks assignment.

Now, let's get notebooks to work. There's a few reasons why we weren't able to run our notebooks, so let's try to set things up properly. I've attached a video that goes through the process visually (click on the image below), but written instructions are also provided below.

[![YouTube](http://i.ytimg.com/vi/BZCkYN2GDHU/hqdefault.jpg)](https://www.youtube.com/watch?v=BZCkYN2GDHU)

First, open up vscode. If you are able to use 
```
code . 
```
that's great! If not, please come talk to us before or after class. If this doesn't work for you, please add a comment to your assignment with the error that you get (a screenshot would be great). Then, open VSCode manually.

Next, open the intro2python folder by clicking open folder. Once you've done this create a new file, with the extention `.ipynb`. You can see in the video that I do this automatically, but it's alright if this doesn't work for you. Just make sure to rename the file so that it ends with `.ipynb`. Once you've done this, it will be important to tell VSCode to use Python. To do this, we will select a python interpreter by typing in control-shift-P (on mac, command-shift-P) to open up the command palette on the top. We can then scroll through and find `python: select interpreter`. Once you've clicked on this, select the intropython environment. You can now try to run a line of code in the notebook you've created (see an example in the video), and it may prompt you again to choose a kernel. Click on intropython again, and you should be able to run the code. NOTE: you may run into an issue where VSCode asks you to install some extentions. Go ahead and do this, and then restart VSCode.

#### DELIVERABLE 2: Please submit a screenshot of the working notebook after you run a cell of code. If it does not work, please email us so we can troubleshoot.

## Optional Extra Work and Resources
### Video on conda and jupyter notebooks

[Video linked here](https://www.youtube.com/watch?v=LCOINLVBVmM)

### Optional extra credit work:
1. Create and run a jupyter notebook, ensuring you have selected the “intropython” environment kernel

2. Create and run 3 cells, making sure none of them output errors:

i. markdown cell
```
# hello world
```

  ii. code cell 

      print(‘hello world’)

  iii. code cell 

      import numpy

3. Take a screenshot of the notebook after executing all the cells, showing that there are no output errors and that you have the correct environment kernel selected. **Include in your Week02/HW1 coursework assignment for extra credit.**

Like last week, if you run into issues please contact us before class. Please upload a screenshot of the problem you are running into to the relevant assignment on courseworks so we can help you debug.





### 1. Download the IntroPython1.ipynb file from this repository folder (Week02).
Please save it in your intro2python folder.
### 2. Commit the  IntroPython1.ipynb to your own intro2python repository.
Feel free to do it via Visual Studio Code or via git. I won't put instructions here on the exact commands, so try to jog your memory (or revisit the slides)!
### 3. Take a screenshot of your intro2python repository with the IntroPython1.ipynb and upload it to the Courseworks Assignment.


## Resources
- [W3 schools python intro](https://www.w3schools.com/python/python_operators.asp)
- [Python's tutorial](https://docs.python.org/3/tutorial/introduction.html)
- [Git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [More on markdown (for jupyter notebooks) in case you are curious](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html)
- [Markdown Cheat Sheet](https://sqlbak.com/blog/wp-content/uploads/2020/12/Jupyter-Notebook-Markdown-Cheatsheet2.pdf)

## Optional After Class Practice
- [Coding Bat](https://codingbat.com/python)
