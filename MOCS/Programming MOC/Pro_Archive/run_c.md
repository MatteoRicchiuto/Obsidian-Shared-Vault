
Tag:[[Unix Terminal MOC]], [[My_Terminal_Scripts]]

---

```terminal
run_c.h programame.c
```

This script is a simple way to compile and run a C program from the command line. If no arguments are passed to the script, it prints a usage message. Otherwise, it compiles the specified source file, runs the resulting binary file, and then removes the binary file.

```bash
#!/bin/bash

if [ $# -eq 0 ]; then
	echo "Usage: $0 <source_file>"
	exit 1
fi

source_file="$1"
binary_file="${source_file%.*}"

gcc "$source_file" -o "$binary_file" && ./"$binary_file" && rm "$binary_file"
```

---
## Explanation
Here's a line-by-line explanation of what this shell script does:

```bash
#!/bin/bash
```
This line specifies the interpreter to use for running the script. In this case, it's `bash`.

``` bash
if [ $# -eq 0 ]; then
	echo "Usage: $0 <source_file>"
	exit 1
fi
```
This block of code checks if the script was called with any arguments. If the number of arguments (`$#`) is equal to 0, it means no arguments were passed. In that case, the script prints a usage message that includes the name of the script (`$0`) and exits with an error code of 1.

``` bash
source_file="$1"
binary_file="${source_file%.*}"
```
These two lines set the `source_file` variable to the first argument passed to the script (`$1`). The second line sets the `binary_file` variable to the same name as the source file, but with the extension removed. This is done using parameter expansion: `${source_file%.*}` removes the shortest match of `.*` (i.e., the file extension) from the end of the `source_file` variable.

```bash
gcc "$source_file" -o "$binary_file" && ./"$binary_file" && rm "$binary_file"
```
This line does three things:

1. It compiles the source file (`$source_file`) into an executable binary file with the same name as the source file (but without the extension) using `gcc`. The `-o` option specifies the output file name (`$binary_file`).
2. If the compilation is successful (i.e., if `gcc` returns a zero exit code), it runs the binary file using `./"$binary_file"`.
3. Finally, it removes the binary file using `rm "$binary_file"`.

So overall, this script is a simple way to compile and run a C program from the command line. If no arguments are passed to the script, it prints a usage message. Otherwise, it compiles the specified source file, runs the resulting binary file, and then removes the binary file.