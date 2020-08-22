# Read & Write Files in Python

**Files on most modern file systems are composed of three main parts:**

* Header: metadata about the contents of the file (file name, size, type, and so on).

* Data: contents of the file as written by the creator or editor.

* End of file (EOF): special character that indicates the end of the file.

**File Paths**

>When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file.

* Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows).

* File Name: the actual name of the file.

* Extension: the end of the file path pre-pended with a period (.) used to indicate the file type.

# Exceptions in Python

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception. In this article, you will see what an exception is and how it differs from a syntax error. After that, you will learn about raising exceptions and making assertions. Then, you’ll finish with a demonstration of the try and except block.

>raise allows you to throw an exception at any time.

>assert enables you to verify if a certain condition is met and throw an exception if it isn’t.

>In the try clause, all statements are executed until an exception is encountered.

>except is used to catch and handle the exception(s) that are encountered in the try clause.

>else lets you code sections that should run only when no exceptions are encountered in the try clause.

>finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.