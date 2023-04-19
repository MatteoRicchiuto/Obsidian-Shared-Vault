Tag:[[Unix Terminal MOC]]

---

# rm use cases
The `rm` command is used to remove files or directories from the file system. Here are some common use cases for the `rm` command:

1. **Deleting a single file:**
	-  For example, `rm myfile.txt` will delete the file named `myfile.txt` from the current directory.

2. **Deleting multiple files:** 
	- You can use wildcards to delete multiple files that match a pattern. For example, `rm *.txt` will delete all files with a `.txt` extension in the current directory.

3. **Deleting a directory:**
	- You can use the `-r` option with `rm` to delete a directory and its contents recursively. For example, `rm -r mydir` will delete the directory named `mydir` and all files and subdirectories within it.

4. **Forcefully deleting files:** 
	- By default, `rm` will prompt you before deleting each file to confirm that you want to delete it. You can use the `-f` option to force `rm` to delete files without prompting. For example, `rm -f myfile.txt` will delete `myfile.txt` without prompting.

5. **Deleting files owned by another user:** 
	- If you have sufficient permissions, you can use `rm` to delete files owned by another user. For example, `sudo rm otheruser/myfile.txt` will delete `myfile.txt` from the home directory of `otheruser`.

---
# How to delete a binary file after running it
you can use the `rm` command to delete the binary file after running it. 

Here's an example command that compiles and runs the program, and then deletes the binary file:
```
gcc H_Ex27.c -o H_Ex27 && ./H_Ex27 && rm H_Ex27
```
This command uses the `&&` operator to chain multiple commands together. The `gcc` command compiles the source code and creates the binary file. The `./H_Ex27` command runs the program. Finally, the `rm H_Ex27` command deletes the binary file.

>[!note]
>If you want to run this command frequently, you can create a **shell script** file with this command and execute the script whenever you want to run the program.

