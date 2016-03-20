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

## Conclusion

I hope this does look good on GitHub, and that I didn't do to many spelling mistakes. No much hope about the later... 