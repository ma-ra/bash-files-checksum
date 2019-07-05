# bash-files-checksum 
```
!!! Alpha Version

Program to detect changes in the files, for example in case of failure hard drive.
Use:
   fc init      - create repository; count checksums for all files
   fc update    - recalculates the checksum for all files
   fc status    - show changes between "init/penultimate update" and "last update"; list modified, added and deleted files
   bfc bfcless  - run on parent directory; show directories that not containt .bfc subdirectory
   bfc updstat  - run on parent; show last update date
   bfc updstat - run on parent directory; show last update
   bfc dup [current1.sum] [current2.sum] - run on parent directory; find duplicate files by hash
   bfc dup -files current1.sum current2.sum - run on selected files; find duplicate files by hash
Example:
   update all - for i in * ; do echo -e "\n$i" ; bash -c "cd \"$i\" && bfc update" ; done
```
