## Basic Linux Shell Commands and Utilities

###### mkdir - create directory

```shell
mkdir mydirectory
```

###### cd - change current directory

```shell
cd mydirectory
```

###### touch - create an empty file

```shell
touch file.txt
```

###### ls - list directory

```shell
ls #list directory
ls -l #list by author
ls -t #list by time
ls -sSh #list by size
```

###### clear - clear the terminal screen

```shell
clear
```

###### man - an interface to the reference manuals

```shell
man ls #manual of ls
```

###### head - output first part of the file

```shell
head file.txt #output first 10 lines
head -n 5 file.txt # output first 5 lines
```

###### tail - output last part of the file

```shell
tail file.txt
tail -n 5 file.txt # output last 5 lines.
```

###### less - view file

```shell
less file.txt # open file in read mode.
```

###### cat - concatenate files and print on the standard output

```shell
cat file.txt #print file.txt
cat file1.txt file2.txt #print both file1.txt and file2.txt to standard output
```

###### cp - copy files and directories

```shell
cp file.txt file2.txt #copy file.txt to file2.txt
cp mydirectory newdirectory #copy my mydirectory to newdirectory
```

###### mv - move/rename files and directories

```shell
mv file.txt file1.txt #file.txt renamed to file2.txt
```

###### rm - delete file or directory

```shell
rm file2.txt #file.txt removed
rm -r mydirectory # -r option for directory.
```

###### find - search for files and directory in a directory hierarchy

```shell
find . -name file.txt #search for file or directory name file.txt in current directory
					  # . stands for current directory
find . -name file.txt -type -f # search for a regular file in current directory.
find . -size +1000c #find all files greater than 1000bytes 
find . -size +1k #find all files greater than 1kb in current directory
```

###### grep - print lines matching a pattern

```shell
grep "Hello" file.txt #search for 'Hello' in file.txt
grep "hello" file.txt -i #search for 'hello', -i Ignore case
grep "hello" *  -i #search for 'hello' in all files in current directory
```

###### echo - display a line of text

```shell
echo "hello"
```

###### sort - sort lines of text files

```shell
sort file.txt
```

## Utilities

###### > - redirect output to a file.

```shell
echo "hello" > file.txt # write "hello" to file.txt. Overwrites file.
```

###### >> - append output to a file.

```shell
echo "hello2" >> file.txt # append "hello2" to file.txt.
```

###### | - pipe - set of commands chained together

```shell
ls | less #list directory and view output in less
ls | sort | head -n 4 #list directory, then sort , then print first 4 lines of sorted output
ls | sort | head -n 4 | tail -n 2 #guess it!
```

#### VIDEO

[Linux Shell Basics](https://www.youtube.com/watch?v=MlTrftsAjyE)

