# datasciencecoursera

Author : Dylan Tweed
Date   : 03/20/2016

## Content and Objective

This is a README for Data Science Course on Coursera
This repo has an extra file HelloWorld.md 
The point of this assignement is to test whether I can create a local repo with a dummy markdown file and put it in a remote GitHub repository

The file HelloWorld.md should in the end contain a single line as a section title
"This is a MarkDown document"

And since I am at it, might as well play with MarkDown while detailling what I did.
Anyway always a good idea to make a README... 

## Assignement Description

It consist on creating both local and remote repo.
The file created on the repo must be written localy and pushed to the remote one. 
Actually it would be easy to do the remote repo, and create the HelloWord.md file there, but 
quite realistically, one would usually either:

* create a repo with git in locally then create a remote copy to be synchronised.
* fork an existing remote repository pull it to its local machine and later submit changes

## Setting the repo on my local machine

So let make the repo first:

1. Create a new directory datasciencecoursera: $mkdir datasciencecoursera
2. Go to the new directory with: $cd datasciencesoursera
3. Create and edit this file HelloWorld.md: $emacs -nw HelloWorld.md
4. Next create the git repo with: $git init

## Creating the remote copy repo

Well this part is obviously from my web browser.

1. I logged to my GitHub account
2. Created a new repository called datasciencecoursera
3. I didn't tick the box with Initialize this repository with a README, the cloning might be tricky with the README.md on the remote repository and the local with this file.

That is interesting, GitHub notice I didn't initialize, so it kindly tells me what to do on my local computer. That is quite considerate.

## Back to my local machine

Well now I will simply be lazy and follow the intruction provided by github.
Namely

1. $git init \#already done that so the change I made to this file should be commited
2. $mv HelloWorld.md README.md \# This text is better as a README to limit the HelloWorld.md to the assignment.
3. $git add README.md \#That is just to add the new file to the repo 
4. $git commit -m "first commit" #Well just commiting the new change, new README.md and HelloWorld.md
5. $git remote add origin https://github.com/BreaizhZut/datasciencecoursera.git \# That just associate the remote repo url to the local repo
6. $git push -u origin master \# Simply upload my local repo content to the remote server as the master branch 

What I did forget is to add the HelloWorld.md to the repo. The reason why is that I though this file that I created prior to doing the git init would be added to the repo. That is good to know, the repo is empty at initialization whatever files are coantained in the directory.
So That is good I now have to do the following

1. $git add HelloWorld.md
2. $git commit -m "Second commit. Adding the missing HelloWorld.md and edited README.md"
3. $git push origin master

Once again something went wrong, it is good to have added the new file and it worked perfectly but, the commit didn't take into account the changes I made to this README.md. 
So it seem any changes need to be staged before commit.
Meaning git add must be run on each file before a commit.

1. $git status \#Tell me whether my working directory is up to date, let me know if some file were edited and not staged
2. $git add README.md 
3. $git status \# Should confirm that the latest changes to this file were staged
4. $git commit -m "" \# Now that all changed are staged I can commit
5. $git status \# Should now not list any changes to be commited
6. $git diff \# show all differences from the master branch should show nothing
7. $git push -u origin master \# Should get this mess sorted once and for all

## Conclusion

I hope this does look good on GitHub, and that I didn't do to many spelling mistakes. No much hope about the later... 