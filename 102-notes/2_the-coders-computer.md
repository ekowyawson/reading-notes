# The Coder's Computer

The command Line Interface (CLI) is a bare text-based interface that allows a computer user to input commands that directly interact with the computer operating system (OS). A person can use the CLI to do pretty much everything that can be done using the computer's visual graphical user interface (GUI); i.e., using the mouse and keyboard to click icons. However, the CLI can do much, much more and much, much faster!

Text editors programs (whether CLI-based or GUI-based) that allow you to create, save, and edit text files on your computer. It is important not to confuse CLI and text editors. Let's briefly delve into these concepts.

## What are four important features to look for in a text editor?

There are tons of different text editors out there to choose from. Most are free to download but there are some that are subscription-based. Ultimately, the one to choose boils down to what you are most comfortable with. With that said, there are some basic features of text editors that I recommend every software / web developer pay attention to when deciding on which one to choose. Below are four of these features:

1. **Code completion** - allows you to press ```Tab``` or ```Enter``` to complete your code based on the coding language (i.e., JavaScript).
2. **Syntax highlighting** - highlights specific code verbiage for easier reading and editing.
3. **Linting** - a special feature of some text editors that underlines and changes the color of incorrect code or code that breaks best practices.
4. **Extensions** - special programs that allow a multitude of functions when you are coding in specific languages, such as displaying the definition of certain commands and functions.

## What do the following commands do?

1. **pwd** - print working directory: displays the full path to the directory that you are currently working in
2. **ls** - list: lists the files and folders within your current directory (or the directory you type after a space character)
3. **cd** - change directory: changes the current working directory to the directory you type after at least one space
4. **mkdir** - make directory: creates an empty directory inside your current working directory, or creates directories you specify after at least one space
5. **touch** - creates an empty file(s) inside the current working directory, or directory you specify after at least one space

## Explain what is happening in the following scenario if these commands and arguments are entered into the command line?

> *(Arguments are extra instructions given to a command.)*

```bash
cd projects
mkdir new-project
touch new-project/newfile.md
cd ..
ls projects/new-project
```

### The commands above are accomplishing the following tasks in succession:

1. change working directory to the `projects` directory
2. make a new directory inside the `projects` directory called `new-project`
3. create an empty file called `newfile.md` inside the `projects/new-project` directory path
4. change the current working directory, moving backwards one directory (parent directory of `projects`)
5. list the `projects/new-project` directory, which should only show the `newfile.md` file
