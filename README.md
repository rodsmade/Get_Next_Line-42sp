# get_next_line
This project introduces the concepts of _static variables_, _dynamic memory allocation_, _file descriptors_ and _macros_ while solving one simple task: that of using the Linux standard function `read()` to scan a file for _single lines_ (i.e. strings of chars ending in a single trailing `\n` (new line character)).

## Files
* ```get_next_line.c```
	function implementation

* ```get_next_line_utils.c``` 
	auxiliary functions (project requirement)

* ```get_next_line.h``` 
	header file

* ```only_skin``` 
	sample text file (also lyrical masterpiece) for testing purposes. File size: **6940 bytes**; new line char count: **251**.

* ```main.c``` 
	printing loop iterating over the file. calls get_next_line to fetch each line, then prints.

## Run the program
On your terminal, make sure to be on the same level as the *.c files, then run the command:
```c
gcc get_next_line_utils.c get_next_line.c main.c -D BUFFER_SIZE=42 -o get_next_line
```
Here `BUFFER_SIZE` determines the size of the buffer used to read the file (in other words, how manny chars shall be read at once with every `read()` call).
To run the program, enter the following in the command prompt:
```c
./get_next_line
```

You should expect to see the lyrics to Only Skin by Joanna Newsom printed in your terminal window. How cool is that?!

![Ys album cover](ys.png)

## Final note
If you're a 42 student struggling to understand this project, I got your back! Please refer to this Notion page that I wrote covering the general concepts related to this project and a practical to-do list of tasks to help you get started writing your own `get_next_line`! It's in Portuguese :cactus:

[Acelera — Get_next_line](https://rodsmade.notion.site/Acelera-Get_next_line-4902aab835ef4b86a7c55d82cc5c19ec)
