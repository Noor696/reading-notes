## Automation

### Python Regular Expressions Tutorial
[Python Regular Expressions Tutorial](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)

* Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not.

*  They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

* some very useful functions provided by the re library, such as: compile(), search(), findall(), sub() for search and replace, split().

* In Python, regular expressions are supported by the re module. **import re**

* The match() function returns a match object if the text matches the pattern. Otherwise, it returns None.

* the search function, you scan through the given string/sequence, looking for the first location where the regular expression produces a match.

* The group function returns the string matched by the re.



### shutil
[shutil](https://pymotw.com/3/shutil/)

* The shutil module includes high-level file operations such as copying and archiving.

* **Copying Files** copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.

* The implementation of copyfile() uses the lower-level function copyfileobj(). While the arguments to copyfile() are filenames, the arguments to copyfileobj() are open file handles. The optional third argument is a buffer length to use for reading in blocks.

* **Copying File Metadata**
By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

* **Working With Directory Trees**
shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

* **Finding Files**
The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

* **Archives** Python’s standard library includes many modules for managing archive files such as tarfile and zipfile. There are also several higher-level functions for creating and extracting archives in shutil. get_archive_formats() returns a sequence of names and descriptions for formats supported on the current system.

* **File System Space** It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.

### Super quick Python automation ideas
[Super quick Python automation ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)

### Al Sweigart, "Automating Your Browser and Desktop Apps"
[Al Sweigart, "Automating Your Browser and Desktop Apps", PyBay2016](https://www.youtube.com/watch?v=dZLyfbSQPXI)

