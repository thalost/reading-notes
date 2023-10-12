
## Class 2 Reading Notes

### Review Questions

## 1. What are four important features to look for in a text editor?

Answer: 
A text editor is a software application used for creating, editing, and managing plain text files. It is a fundamental tool for programmers, developers, writers, and anyone working with text-based files, including code, scripts, configuration files, documentation, and more.




## 2. What do the following commands do?
pwd
ls
cd
mkdir
touch

Answer:
pwd (Print Working Directory): This command displays the current directory or folder that you are in. It shows the full path to your current location in the file system.

ls (List): The ls command is used to list the files and directories in the current directory. When used without any options, it provides a basic list of files and directories.

cd (Change Directory): The cd command is used to change the current directory or navigate to a different directory. You provide the directory's name or path as an argument to cd.

mkdir (Make Directory): This command is used to create a new directory or folder within the current directory. You specify the name of the directory you want to create as an argument to mkdir.

touch: The touch command is used to create a new, empty file. It can also be used to update the access and modification times of an existing file. To create a new file, you provide the file's name as an argument to touch.

These commands are fundamental for interacting with the file system and navigating directories in a command-line environment.









##  3. Can you explain what is happening in the following scenario if these commands and arguments are entered into the command line? (Arguments are extra instructions given to a command.)
cd projects
mkdir new-project
touch new-project/newfile.md
cd ..
ls projects/new-project

Answer: 


cd projects: This command changes the current directory to a folder named "projects."

mkdir new-project: This command creates a new directory or folder named "new-project" within the "projects" directory.

touch new-project/newfile.md: This command creates a new file named "newfile.md" within the "new-project" directory. The touch command is used to create an empty file.

cd ..: This command changes the current directory to the parent directory of the current location. In this case, it moves you up one level from "new-project" to the "projects" directory.

ls projects/new-project: This command lists the contents of the "new-project" directory within the "projects" directory. It will display the file "newfile.md" if it was successfully created in step 3.

Here's a summary of what's happening:

You navigate to the "projects" directory.
You create a new directory called "new-project" inside "projects."
Inside the "new-project" directory, you create a new file named "newfile.md."
You then navigate back up to the "projects" directory.
Finally, you list the contents of the "new-project" directory to verify that "newfile.md" exists.
This sequence of commands and arguments is creating a new project directory structure and verifying the file creation within that structure.
