# GITHUB


Git is a distributed version control system (DVCS)  for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files.

There are three areas where information is stored in Github.  1 local working directory 2 staging area 3 online repository.  Files can be modified on a local machine, then a 'snapshot' can be committed to the staging area, and then the 'snapshot' can be pushed from the staging area and the changes added to the repository.

Several commands are useful when working with the files in Terminal:

- Track one file only by using the following format: git add filename

- Track all files in a repository by using the following command: $ git add *

- See information regarding changes to be committed when using the git status command: $ git status

- Committing a File: $ git commit -m “made change x,y,z” with a message on what changes were made

- Committing All Changes: $ git commit -a

- Pushing Changes: $ git push origin master
