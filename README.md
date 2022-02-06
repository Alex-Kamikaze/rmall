# rmall
> version 1.0.2
A simple programm, inteneded to replace "rm" and "rmdir" by combining their features in single executable.

## Installing
>Windows
You can install programm by cloning repo to your local machine, and then add directory, which contains executable, directly to PATH variable. 
>Linux
To install Linux version, follow the same steps, but then move binary executable to usr/bin directory.

## Quickstart
Just open terminal and then type:
< rmall dir >
Where dir - directory, which should be deleted. rmall also can delete files, for example:
< rmall dir_1 file.txt >
rmall will delete dir_1, when will try to delete file.txt as a directory, and will get an error, then util will try to delete it as a file, and this will be succesfull.

## Source code
The program is entirely written in Rust programmming, cause Rust provides great perfomance and have an amazing ecosystem with cool package manager called Cargo. In previous versions of Rust, the vulnerability CVE-2022-21658 can be used to delete system folders using the standard library function, but rmall is compiled using rustc version 1.58.1, which fixes this vulnerability, so rmall cannot be used by attackers. 
