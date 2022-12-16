# Group 6 - HW3

## 1-

13504616

## 2-

Yes

## 3-

its identical

## 4-

Yes, its identical

## 5-

Yes

## 6-

Strace traces system calls and signals. In the simplest case Strace runs the specified command until it exists. Strace is a useful *diagnostic*, *instructional*, and *debugging tool*.

## 7-

 The rm command removes references to objects from the filesystem using the ****unlink**** system call

<img title="" src="https://i.imgur.com/gaN7MFA.png" alt="1.png" data-align="center">

## 8-

It is unique

## 9-

Yes

## 10-

The file is empty but after adding some text and saving it the oslabfile3.txt file will get created again.

<img src="https://i.imgur.com/ee6CpEr.png" title="" alt="1.png" data-align="center">

## 11-

**Hard Link :** 
A hard link acts as a copy (mirrored) of the selected file. It accesses the data available in the original file. 
If the earlier selected file is deleted, the hard link to the file will still contain the data of that file.

**Soft Link :** 
A soft link (also known as Symbolic link) acts as a pointer or a 
reference to the file name. It does not access the data available in the
 original file. If the earlier file is deleted, the soft link will be 
pointing to a file that does not exist anymore.

**differences:**

- symlinks can cross file systems, hard links can't. If you delete the original file, the hardlink still keeps it alive, a symlink doesn't.

- A hard link essentially means the file lives in two places, it can have different permissions, you can delete it in on place but not the other.

- A soft link is just a pointer to the real thing.

**Inode number :** 

Index node number is a unique number assigned to all files in a Linux/Unix system.

<img src="https://i.stack.imgur.com/f7Ijz.jpg" title="" alt="f7Ijz.jpg" data-align="center">

## 12-

for example assume that you have a large collection of video files on your external hard drive (or on another internal drive) that you want to access frequently and you don't have the space to store it on your internal (or main) storage you could simply *symlink* your video folder from your external hard drive to your video folder from your internal storage. It allows you to have multiple "access points" to a file, without having excess copies (that remain up to date, since they always access the same file).

Note: A hard link can only reside on *the same* filesystem as the file it's pointing to.
