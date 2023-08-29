# INTRODUCTION TO SHELL SCRIPTING.

`ls` -**is a command used to list files in your current working directory**.


It can be used with different flags (***flavors***) to modify the search to your liking.


***Examples***

`ls -a`  can be used to list all files including files with a dot.

In linux files with a dot are ***hidden*** files.


`administrator@administrator-Legion-5-15IAH7:~/shell-lesson-data$ ls`

`exercise-data   file.txt  north-pacific-gyre   projects  trial_2.txt`

In this example when we just use `ls` we can see the files listed here are not hidden.

`administrator@administrator-Legion-5-15IAH7:~/shell-lesson-data$ ls -a`

`.  ..  exercise-data  file.txt  .latifah  north-pacific-gyre  projects  trial_2.txt`

We can see the difference here when we use the command `ls -a` because we can see the file .Latifah. 🔥 🔥


`ls -r` is a flag used to list files in reverse order while sorting.

`administrator@administrator-Legion-5-15IAH7:~/shell-lesson-data$ ls`

`exercise-data  file.txt  north-pacific-gyre  projects  trial_2.txt`

Note how the files are listed when we just use the `ls` command.

`administrator@administrator-Legion-5-15IAH7:~/shell-lesson-data$ ls -r`

`trial_2.txt  projects  north-pacific-gyre  file.txt  exercise-data`

Can you see the difference now? 🤔

The list is now **REVERSED**







