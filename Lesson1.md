In this lesson we will give you command examples.  After typing the command, press Enter to execute.

Welcome to Lesson 1.  Do you know what your current working directory is?  Let's find out.  Type the command:

    $ pwd

Did the command show you output similar to "/home/yourname" where "yourname" is the username you signed up with? Congratulations,you have found your current working directory and have joined exclusive club of linux commandline users!

For the next command we will need your current working directory to be your home directory.  Type the command:

	$ pwd
	
If you are not in your home directory, type the command:

	$ cd
	
Now lets try to create a new directory.  Type the command: 

    $ mkdir -v dir1

Did your command prompt output:

	mkdir: created directory dir1

Way to go! You just created a new directory. Lets say you want to create more than one directory.  You could type the command multiple times:

	mkdir -v dir2
	mkdir -v dir2/dir3
	mkdir -v dir2/dir3/dir4

Or you can take a smart shortcut and type the command: 

	$ mkdir -vp dir2/dir3/dir4

The "-p" option will create all of the parent directories for "dir4".  In this case,it created 

	dir2/
	dir2/dir3/

automatically.  Now that we have created four directories, how do we view them? Type the command:

	$ ls

You may notice that the command is only showing you:

	dir1
	dir2
	
But we made more than that, right?  Right!  Our other directories are inside of:

	dir2
	
The command "ls" is only showing us what is inside our current working directory.  Type the command:

	$ ls -R 

and we should get the output:

	./dir1:

	./dir2:
	dir3

	./dir2/dir3:
	dir4

	./dir2/dir3/dir4:

The "-R" is a command argument or parameter.  For the command "ls" it stands for recursive.  Now that we have created a new directories and listed them,lets move into a new directory.  Type the command:

	cd dir2

You have changed to "dir2".  Lets confirm this.  Type the command:

	$ pwd

Lets move into next directory.  Type the command:

	cd dir3
	
And now we are in the "dir3" directory.  But what if we needed to go back?  Type the command: 

	$ cd ..

We have moved to the parent directory, which is "dir2".  We are finished with working in this directory, so let's go back to the previous working directory.  Type the command:

	$ cd -

We are now back in the directory "dir3".  Do you feel like a linux commandline pro yet?  Let's go back home.  Type the command:

	$ cd

We have returned to your home directory.  That's it, You have successfully completed lesson 1!  Now to start next lesson.