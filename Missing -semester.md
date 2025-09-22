
## echo 
echo : a shell built-in command 
used to print the things you input 

to print multiple words
to quote it 
 **echo " Hello World"**
 
## use a slash to divide the sentence

echo hello\ world



## Variables

a critical variable is $PATH.


**PWD** :print working directory

**cd**:change directory

**.** :  current directory

**..** : parent directory

```bash
ls
```
list the files in the dir you're in 


```bash
cd ~
```
bring you to your home dir

```bash
cd -
```

cd to the dir you were previously in

if you want to find some command :

use 
```bash
man ls
```
to list the files and directories (not hiden)

if you want to list all the files and directories in the dir

use 
```bash
ls -a
```
if you want to list **all files and directories** in the current directory, including **hidden files**, and it provides **detailed information** about each file or directory.
use 
```bash
ls -la
```

if you want to some detailed information about each file or directory, such as permissions, owner, file size, last modification time, and the name of the file/directory.
use 
```bash
ls -l
```


```bash
rm <files_name>
```
to remove the files

```bash
mv food.md vaults.md 
mv <source> <destination>
```

move the file to another place

```bash
cp dot.md food.md
cp <source> <destination>

```

it also gets two arguements
dot.md is where you copy to, food.md is where you copy from

for instance if you want to add sth to a file

```bash
echo <filename> >> <destination>
```

if you want to o **display the contents of a file** on the terminal. It's short for "concatenate," and while its primary purpose is to show the contents of files, it can also be used for a few other things.

use 
```bash
cat <file_name>
```

