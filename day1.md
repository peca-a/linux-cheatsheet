# 📅 Day 1 – Linux Basics

## 📁 Navigation

### cd

* Change directory

Examples:
cd Desktop
cd ..
cd ~

---------------------------------------------------------------------------------------------

### ls

* List directory contents

ls
ls -a
ls -l

---------------------------------------------------------------------------------------------

### pwd

* Show current path

---------------------------------------------------------------------------------------------

## 📂 File & Directory Management

### mkdir

* Create directory

mkdir test
mkdir -p dir1/dir2

---------------------------------------------------------------------------------------------

### rm

* Remove files or directories

rm file.txt
rm -r folder

---------------------------------------------------------------------------------------------

### rmdir

* Remove empty directory

---------------------------------------------------------------------------------------------

### cp

* Copy files

cp file1 file2
cp -r dir1 dir2

---------------------------------------------------------------------------------------------

### mv

* Move or rename files

mv old.txt new.txt

---------------------------------------------------------------------------------------------

## 📄 Viewing Files

### cat

* Show file content

cat file.txt

---------------------------------------------------------------------------------------------

### more

* View file page by page (only forward)

---------------------------------------------------------------------------------------------

### less

* Better file viewer

Controls:

* /word → search forward
* ?word → search backward
* q → quit

---------------------------------------------------------------------------------------------

## 🔍 grep

Search for text inside files

grep error *.log

* Find "error"

grep -i error *.log

* Ignore case

grep -v info *.log

* Exclude "info"

grep -r error .

* Recursive search

---------------------------------------------------------------------------------------------

## 🔢 sort

sort file.txt

* Sort lines

sort -r file.txt

* Reverse sort

sort -u file.txt

* Remove duplicates

---------------------------------------------------------------------------------------------

## 🔗 Redirection

> overwrite file
>
> > append to file

Example:
echo "hello" > file.txt
echo "world" >> file.txt

---------------------------------------------------------------------------------------------

## 🔄 rsync

rsync -a src/ backup/

* Sync directories
* Copy only changes

Difference:
rsync -a dir backup/
→ creates backup/dir

rsync -a dir/ backup/
→ copies content

---------------------------------------------------------------------------------------------

## ⚠️ Common Mistakes

* cd file → works only for directories ❌
* grep * .log → wrong syntax ❌
* missing space after echo ❌
* wrong paths (/ vs relative)

---------------------------------------------------------------------------------------------
