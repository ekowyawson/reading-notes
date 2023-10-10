## What Is Git
Whether you are new to the "developer world" or a seasoned veteran, you have undoubtedly heard about Git and the technology behind it. 
In this short blog, we will discuss what Git is along with a few of its concepts.

So, what is Git? Git is simply a `version control` system for files. The term `Version Control` refers to a technology that tracks changes 
in a file, or set of files, and allows authorized users to revisit and view all changes to those files; thus, allowing those users to view 
progression or revert any mistakes.

The technology was created in 2005 by `Linus Torvalds`, the creator of Linux, along with a few other members in the Linux development 
community, to address code versioning issues at the time.[1] The problem they sought to solve was how to enable large-scale 
collaboration in development efforts, which Git successfully addressed.

## Key Concepts
1.	What is Version Control?
* Version Control is a technology that makes it possible for users and teams to track a file or sets of files by recording changes to those files (versions).
Version Control makes it possible to:
    * Revert to a known better state for code.
    * View who has made changes and what those changes are.
    * Quickly patch bugs found in code.
2.	What is `cloning` in Git?
* Cloning in Git quite literally refers to the cloning of a Git repository (a set of files) stored in a particular server or on a host of servers (cloud).
3.	What is the command to track and stage files?
* To track and stage a file(s) in Git, you would use the following two commands (first one is to track a single file, the second is to track all files in the current repository):
```bash
git add ${filename}
git add *
```
4.	What is the command to take a snapshot of your changed files?
* To take a snapshot of your changed files, you would use the following command:
```bash
git commit -a
```
5.	What is the command to send your changed files to Github?
* To send your files to GitHub, you would use the following command:
```bash
git push origin master
```
## Conclusion
Git is a must have tool for any serious / professional developer. It is also very beginner friendly. No go Git’in!

## Reference
[1] [What is the Git version control system? – TechTarget Definition](https://www.techtarget.com/searchitoperations/definition/Git#:~:text=The%20history%20of%20Git,requirements%20for%20Linux%20kernel%20development.)
