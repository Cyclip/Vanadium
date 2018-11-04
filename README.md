# Vanadium
A python module; when you don't want to reinvent the wheel. Mainly for beginners for Python. Vanadium contains many different functions that beginners would search for, such as how to send an email or download something or a webpage from the internet. All of this is accessible easily, and enables threading inside the vanadium module.

**Python 3.6 is supported. Only tested on Windows.**

## Getting started
To install vanadium, you need pip; which is most likely already installed along with Python.

1. Open Command prompt (search 'cmd')
2. Type `pip install vanadium`
3. Done!

### Prequisites
There are a variety of modules you'll need to install if `pip` doesn't install them.

## Usage
First of all, you'll need to import vanadium. As the name is long, you can do:
`import vanadium as vdm`
If the module imports normally without errors, you're ready to use it.

## Features
Here is a full list and explanation of each function and class.

#### *vdm.generate(length)*
Generates a number code with 5 letters, and a `-` in between. This will repeat for your length. Example:
```
>>> print(vdm.generate(3).code)
1778-6851-8069
```
#### *vdm.get_output(command)*
Gets the output of a command, like in subprocess. There will not be a console and to get the output, use .command. Example: 
```
output = vdm.get_output('net view').command
very long output
```
#### *vdm.getforeground()*
Gets the current foreground/active window. Name of the window is saved to .command. Example:
```
>>> foreground = vdm.getforeground().window
''*Python 3.6.5 Shell*'
```
#### *vdm.joinlist(list_variable, by=None)*
by is optional. It joins a list and converts it to a string. String is at .string. Example:
```
>>> list = ['hello', 'there']
>>> print(vdm.joinlist(list).string)
'hello there'
```
#### *vdm.hashfile(file_path)*
Gets the md5 hash (other hashes will be supported in later versions) of file_path. The file_path should be the path to the file, not the directory. Example:
`vdm.hashfile('C:/Path/to/file.exe')`

#### *vdm.sdownload(url, file_name)*

# Updates

# Todo
- Support other hashes for hashfile
