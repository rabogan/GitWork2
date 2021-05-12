# GitWork2
Getting used to using .gitignore
In essence, this follows the Git/Github section from Angela Yu's Web Development course.

I was pleased to see that the files (and the .gitignore files) uploaded successfully.

That said, I will need to work out how to deal with the "Tell Me Who You Are" issue; which, while easily solved, is a slightly time-consuming.

In addition, the .gitignore file itself has a few memorable traits:
1)  We simply add the file names into the file, on separate lines...for those files we wish to NOT commit
2)  Use the pound/hash key, #, to add comments in a smooth way
3)  It's not difficult to avoid uploading all files of a specific type.  Using * (asterisk) will work.   e.g.  *.txt will prevent all files of type .txt from being uploaded,
should you include it in the .gitignore file

Remember!
You can find 'secret' files using ls -a

$ touch .gitignore CREATES a file.  In Windows, you'll use
$ attrib +h .gitignore   (this makes the file .gitignore a HIDDEN file)
$ start .gitignore (this opens that file)

Other things of note:
git init   //Initialises an empty git repository inside our directory
git add .   //NOTE THE DOT!   Adds all files inside the directory to the Staging Area
git add specific.txt   (Adds a specific file ;))
git rm --cached -r .    //Note the Dot again!   This command removes ALL files from the Staging Area

git remove add origin https://...  THIS LINE tells the local Git repository that we created a remote repository!
git branch -M main    //NOT INCLUDED in that course...
git push -u origin main   //This PUSHES (TRANSFERS) our local repository onto our remote repository (which we named origin).  
We have pushed our local repository onto the remote repository (origin), pushing it onto the main branch.   We have pushed our local respository to the remote repository
using that -u flag!   origin is the name of the remote, as dictated by convention :)
master/main are branch names!

git add (Moves files from the working directory to the staging area)
******git commit (Moves a file from the staging area to the local repository)*****
git commit -m "Complete Chapter 1"
git commit has DASH m to give a message.  THIS MESSAGE OUTLINES THE PURPOSE OF THE COMMIT!!!!!
It is customary and convention to use the PRESENT TENSE for the message.
git push (This transfers ALL of those commits in our local repository onto our remote repository on Github

git status (Shows untracked files not yet in the staging area...or just lets us see what is in the staging area)

git log (Allows us to see our commits)   The extremely long hashes uniquely identify each commit.

git checkout (Would, if we choose, allow us to revert/roll back to the last position in our local repository

git diff "Chapter1.txt" allows us to see the differences between one version of a file and another.
