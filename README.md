## Getting started

* Installing Python + Editors
* Basic shell commands
* Basic git

&nbsp;
&nbsp;

### Installing Python

To install you visit https://www.python.org go to downloads and get the latest version for your particular system.

Python comes with its own default shell with a stand alone GUI which you can check out after installation. If you search for "idle" in your start menu or Mac search box and open the first result, you'll see what it looks like. In this environment you work line by line; you type your command, e.g. `2+2` hit enter, and it returns the result. 

Usually, however, you'd want to work in an editor. If you go "File > New File" from the shell you'll open the python's default editor. As you type in your code, e.g. `print("Hello World!")` it colors different python objects, commands, etc., making it easier for you to read your code. It doesn't autocomplete. To run your code you go to  "Run > Run Module."

You may choose to work in the default shell + editor combination. However, there are other editors you may choose from. Atom is one of them for example. To install you visit https://atom.io and download the version for your particular system. It's a free lightweight editor, it autocompletes your code for you, and has many other advantages. When you open Atom, save your file with a .py extension, e.g. "filename.py" and you're ready to go.

&nbsp;

### Basic shell commands

Shell, as you've probably guessed by now, is an environment where you do things by typing in commands for your machine to run. Shell is your command prompt cmd.exe or PowerShell in Windows or Terminal in Mac. When coding, It's quite useful to know some of its basics.

In MacOSX / Linux Search for `terminal` and open it. In windowd search for `cmd` or its newer version `PowerShell` and open it. Try typing in some of these.


**Print working directory; show it's path** (directory is another name for folders)

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

**Clear the creen**

in MacOSX/Linux Terminal
```
clear
```
in Windows cmd or PowerShell
```
cls
```

**Search for a something in a text file, e.g. .txt or .md**

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

### Basic git


