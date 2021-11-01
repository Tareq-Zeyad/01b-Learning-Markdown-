## **FileIO & Exceptions**
## **Read & Write Files in Python:**
![file](https://www.softwaretestinghelp.com/wp-content/qa/uploads/2018/10/write_data_to_file.png)
### *What Is a File?*
### A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.
<br>

### File three main parts:
- ### **Header**: metadata about the contents of the file (file name, size, type, and so on).
- ### **Data**: contents of the file as written by the creator or editor.
- ### **End of file (EOF)**: special character that indicates the end of the file.
<br>

### File Paths:
- ### **Folder Path**: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows).
- ### **File Name**: the actual name of the file.
- ### **Extension**: the end of the file path pre-pended with a period (.) used to indicate the file type.
<br>

## **Opening and Closing a File in Python**
![file](https://www.softwaretestinghelp.com/wp-content/qa/uploads/2018/10/close_file.png)
### When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:
### file = open('dog_breeds.txt')
<br>

## **Exceptions versus Syntax Errors**
![error](https://slidetodoc.com/presentation_image/0469b82fc4930b15ca1e9c3a349d4352/image-2.jpg)

### Syntax errors are errors that occur when rules of the used programming language are not followed correctly thus creating an error which forces the program to shut down, on the other hand, Exception errors occur when the code it self is not giving an correct out put, mainly used in TDD process of programming.

## **How can we raise an Exception error ?**
### To raise an exception error We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.