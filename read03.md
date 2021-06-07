# Reading and Writing Files in Python

## What Is a File?

At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files on most modern file systems are composed of three main parts:

1. Header: metadata about the contents of the file (file name, size, type, and so on).
2. Data: contents of the file as written by the creator or editor.
3. End of file (EOF): special character that indicates the end of the file.

![Filediagram](https://files.realpython.com/media/FileFormat.02335d06829d.png)

## File Paths

When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows).
2. File Name: the actual name of the file.
3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type.

## Opening and Closing a File in Python

### Opening a file

When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:

```
file = open('dog_breeds.txt')
```

### closing a file

When you’re manipulating a file, there are two ways that you can use to ensure that a file is closed properly, even when encountering an error. The first way to close a file is to use the try-finally block:

```
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

The second way to close a file is to use the with statement:

```
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```

Most likely, you’ll also want to use the second positional argument, mode. This argument is a string that contains multiple characters to represent how you want to open the file. The default and most common is 'r', which represents opening the file in read-only mode as a text file:

```
with open('dog_breeds.txt', 'r') as reader:
    # Further file processing goes here
```


Other options for modes are fully documented online, but the most commonly used ones are the following:

| Characte      |          Meaning                  ----------------------   |
|---------------|------------------------------------------------------------|
|    'r'        |   Open for reading (default)                               |
|    'w'        |   Open for writing, truncating (overwriting) the file first|
|    'rb'       |   or 'wb' Open in binary mode (read/write using byte data) |



## file object

A file object is:

“an object exposing a file-oriented API (with methods such as read() or write()) to an underlying resource.” (Source)

There are three different categories of file objects:

1. Text files
2. Buffered binary files
3. Raw binary files


## Text File Types

A text file is the most common file that you’ll encounter. Here are some examples of how these files are opened:

```
open('abc.txt')

open('abc.txt', 'r')

open('abc.txt', 'w')
```

With these types of files, open() will return a TextIOWrapper file object:

```
>>> file = open('dog_breeds.txt')
>>> type(file)
<class '_io.TextIOWrapper'>
```

## Reading and Writing Opened Files

Once you’ve opened up a file, you’ll want to read or write to the file. First off, let’s cover reading a file. There are multiple methods that can be called on a file object to help you out:


| Method            |          what is does                                     |
|-------------------|------------------------------------------------------------|
| .read(size=-1)    | This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read |
| .readline(size=-1)|This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read. |
| .readlines()      |	This reads the remaining lines from the file object and returns them as a list.   |


 Here’s an example of how to open and read the entire file using .read():

 ```
>>> with open('dog_breeds.txt', 'r') as reader:
>>>     # Read & print the entire file
>>>     print(reader.read())
Pug
Jack Russell Terrier
English Springer Spaniel
German Shepherd
Staffordshire Bull Terrier
Cavalier King Charles Spaniel
Golden Retriever
West Highland White Terrier
Boxer
Border Terrier
```