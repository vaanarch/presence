## Getting started

* Installing Python + Editors
* Basic shell commands
* Pip and virtual environments
* Basic git

&nbsp;
&nbsp;
&nbsp;

### Installing Python

To install you visit https://www.python.org go to downloads and get the latest version for your particular system.

Python comes with its own default shell with a stand alone GUI which you can check out after installation. If you search for "idle" in your start menu or Mac search box and open the first result, you'll see what it looks like. In this environment you work line by line; you type your command, e.g. `2+2` hit enter, and it returns the result. 

Usually, however, you'd want to work in an editor. If you go "File > New File" from the shell you'll open the python's default editor. As you type in your code, e.g. `print("Hello World!")` it colors different python objects, commands, etc., making it easier for you to read your code. It doesn't autocomplete for you. To run your code you go to  "Run > Run Module."

You may choose to work in the default shell + editor combination. However, there are other editors you can choose from. Atom is one of them for example. To install you visit https://atom.io and download the version for your particular system. It's a free lightweight editor, it autocompletes your code for you, and has many other advantages. When you open Atom, save your file with a .py extension, e.g. "filename.py" and you're ready to code in python. PyCharm is another one of those editors specifically made for python, it's much heavier and has more built-in functionality. If you'd like to use that instead of Atom go to https://www.jetbrains.com/pycharm/ and install the free community version.

&nbsp;

### Basic shell commands

Shell, as you've probably guessed by now, is an environment where you do things by typing in commands for your machine to run. Shell is your Command Prompt cmd.exe or its newer version PowerShell in Windows or Terminal in Mac, and Linux. When coding, It's quite useful to know some of its basics.

In MacOSX / Linux Search for `terminal` and open it. In Windows hit `windows key + R` type `PowerShell` hit enter. You can change that annoying blue color in windows powershell by right clicking on the frame and navigating to the color tab. Try typing in some of these.

&nbsp;

**Run a python code** (same as running a code from the python's stand alone shell and editor)

```
python filename.py
```

**Print working directory; show its path** (directory is another name for folders)

```
pwd
```

**List the content of the current directory**

```
ls
```

**Make a new directory**

```
mkdir NAME_OF_YOUR_DIRECTORY
```

**Change directory**

```
cd NAME_OF_YOUR_DIRECTORY
```

**Go up one directory**
```
cd ..
```

**Open a file (mac only)**

```
open FILENAME
```

**Open the current directory in the Finder (mac only)**

```
open .
```

**Print the contents of a file to the screen**

```
cat FILENAME
```

**Print the contents of a file to the screen, with pagination**

```
more FILENAME
```

**Clear the screen**

in MacOSX/Linux Terminal
```
clear
```
in Windows cmd or PowerShell
```
cls
```

**Search for something in a text file, e.g. .txt or .md**

```
grep 'SearchTerm' FileName
```

**Output your search results into a separate text file**

```
grep 'SearchTerm' File.txt > NewFile.txt
```

**Sort a text file alphabetically**
```
sort FILENAME
```

**Get help/print the manual of a given command**
```
man COMMAND
```

&nbsp;
&nbsp;

### Pip and Virtual Environments

Whenever you want to install additional functionality for python i.e. a library/package you type in `pip install PackageName` in your system's shell. This, however, will download and install the package in your python's systems folder, making it available globally. This might be a problem e.g. when you're using two different versions of python or working with two different versions of the same package for separate projects, etc.. To avoid cluttering your system, you'd want to create a separate folder and place all the files necessary to run your script in that location, including a particular version of the python interpreter. This separate environment where your project lives is referred to as Virtual Environment. 

To create a virtual environment first start your shell (terminal in Mac, powershell in Windows). It'll start in your user's folder which is one folder up from the desktop. Type `pwd` to make sure. Navigate to your desktop or to any other directory by typing `cd desktop`. Now make a new directory for your project `mkdir project-name` then change into the new directory `cd project-name`. Now, when you're inside your project's directory type **`python -m venv ./venv`.** This will create a virtual environment inside that folder, in a subdirectory named `venv`. If your in a Windows powershell type `tree`, if you're in a Mac Terminal type `ls * -r`, these will show all the files and folders that just got created inside that folder.

If you type in `pip --version` however, you'll see that your package installer is still running from the global directory. To activate the virtual environment you've just created and start working from it you need to load a script from inside the venv folder. In MacOSX type `source ./venv/bin/activate`, in Windows `.\\venv\scripts\activate`, now you should see a `(venv)` in the begining of the line, which indicates you're in that particular virtual environment. If you ran into an 'execution policy' error in windows, run your shell as an administrator and type in the following `Set-ExecutionPolicy Unrestricted -Force`, then exit the shell. Now when you open the powershell and change into your projects directory `.\\venv\scripts\activate` command should work.

While your virtual env is active you can type in `pip list` to see the packages installed. For the test type in `pip install beautifulsoup4`to install the beautifulsoup package. Now type in `pip list` again, and you can notice the added package.

To deactivate the venv type `deactivate`. If you're not going to use that folder you can delete it as well.


&nbsp;
&nbsp;

### Basic git


