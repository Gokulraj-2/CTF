## Leviathan

  `Host : leviathan.labs.overthewire.org`
  
  `Port : 2223`


 - level 0 : `bandit0`  

 - level 1 : `PPIfmI1qsA`

In this level they hide a file in the home directory . using `-la` command to show the hidden file list.And then using cat to conacate the contents in bookmarks.html.After that I just searched the word password using grep command to get the password.

 - level 2 : `mEh5PNl10e`

While solving the level they give a setuid executable file . while executing it asks a password.First I entered the previous level password to try.But I says it was wrong password.So I read the content of the executable file using strings command.In the middle of the file it has some bash commands.After that I checked in google and got to know about ltrace.

```bash
leviathan1@gibson:~$ ltrace ./check
__libc_start_main(0x80491e6, 1, 0xffffd6a4, 0 <unfinished ...>
printf("password: ")                                                      = 10
getchar(0xf7fbe4a0, 0xf7fd6f90, 0x786573, 0x646f67password: hlo
)                       = 104
getchar(0xf7fbe4a0, 0xf7fd6f68, 0x786573, 0x646f67)                       = 108
getchar(0xf7fbe4a0, 0xf7fd6c68, 0x786573, 0x646f67)                       = 111
strcmp("hlo", "sex")                                                      = -1
puts("Wrong password, Good Bye ..."Wrong password, Good Bye ...
)                                      = 29
+++ exited (status 0) +++
```

 - level 3 : `Q0G8j4sakn`

While Solving in the level 2, At first I don't have any idea about this level. Then there's a executable file called printfile, then i try to print the `/etc/leviathan_pass/leviathan3`, it says "You cant have that file... ".
then I try to create a file and make symbolic link Then i tried creating a file int the tmp and make symbolic link and printed the file and yeah! I got the answer.
```bash
$ ltrace ./printfile /etc/leviathan_pass/leviathan3
__libc_start_main(0x804852b, 2, 0xffffd764, 0x8048610 <unfinished ...>
access("/etc/leviathan_pass/leviathan3", 4)                         = -1
puts("You cant have that file..."You cant have that file...
)                                  = 27
+++ exited (status 1) +++
```


 - level 4 : `AgvropI4OA`

When I entered in this level there's nothing the home directory, then i started exploring is there any hidden files,there's a folder `'.trash'`. Inside that there a executable file named `bin`, I cat the file its binary file. when I used ltrace.
It's actually reading the password file. when i normally ran the file, it gave me same binary files and i went google searched some binary to text converters. Successfully I am able to find the answer

 - level 5 : `EKKlTF1Xqs`


 - level 6 : `YZ55XPVk2l`

while entering the level it have leviathan6 executable file in home directory.but it shows `usage: ./leviathan6 <4 digit code>`; 
So I run a for loop from `0000` to `9999`.

 - level 7 : `8GpZ5f8Hze`	
