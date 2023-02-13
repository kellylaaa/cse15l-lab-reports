# Lab Report 3

## Researching Commands
##### 1. `find -name`

example 1: This command finds files with the name "ch1.txt" and it's useful because it helps find the file with the searched name.

input: 
```
find . -name "ch1.txt"
```

output:
```
./non-fiction/OUP/Berk/ch1.txt
./non-fiction/OUP/Abernathy/ch1.txt
./non-fiction/OUP/Rybczynski/ch1.txt
./non-fiction/OUP/Kauffman/ch1.txt
./non-fiction/OUP/Fletcher/ch1.txt
```

example 2: This command finds files with the name "ch2.txt" and it's useful because it helps find the file with the searched name.

input: 
```
find . -name "ch2.txt"
```

output:
```
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Abernathy/ch2.txt
./non-fiction/OUP/Rybczynski/ch2.txt
./non-fiction/OUP/Fletcher/ch2.txt
```
---
##### 2. `find -type`
example 1: This command finds files with the file type 'f' (which are regular files) and it's useful because it helps you find all the
files of that type.

input: 
```
find ./non-fiction/OUP/Berk -type f
```

output:
```
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Berk/ch1.txt
./non-fiction/OUP/Berk/CH4.txt
./non-fiction/OUP/Berk/ch7.txt
```

example 2: This command finds files with the file type 'd' (directories) and it's useful because it helps you find all the
directories in the current directory.

input: 
```
find . -type d
```

output:
```
.
./non-fiction
./non-fiction/OUP
./non-fiction/OUP/Berk
./non-fiction/OUP/Abernathy
./non-fiction/OUP/Rybczynski
./non-fiction/OUP/Kauffman
./non-fiction/OUP/Fletcher
./non-fiction/OUP/Castro
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```
---
##### 3. `find -size`

example 1: This command finds files with files with the size less than 100KB and it's useful because it helps you find all the
files that are less than that size.                                 
input: 
```
find ./non-fiction/OUP/Berk -size -100k
```

output:
```
./non-fiction/OUP/Berk
./non-fiction/OUP/Berk/ch1.txt
./non-fiction/OUP/Berk/ch7.txt
```

example 2: This command finds files with files with the size greater than 100KB and it's useful because it helps you find all the
files that are greater than that size.                                                    
input: 
```
find ./non-fiction/OUP/Berk -size +100k
```

output:
```
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Berk/CH4.txt
```
---
##### 4. `find -mtime`

example 1: This command finds files with files that were modified more than a day ago and it's useful because it helps you find all the
files modified after a certain amount of days.  

input:
```
find ./non-fiction/OUP/Castro -mtime +1
```

output: 
```
./non-fiction/OUP/Castro
./non-fiction/OUP/Castro/chR.txt
./non-fiction/OUP/Castro/chP.txt
./non-fiction/OUP/Castro/chQ.txt
./non-fiction/OUP/Castro/chB.txt
./non-fiction/OUP/Castro/chC.txt
./non-fiction/OUP/Castro/chA.txt
./non-fiction/OUP/Castro/chV.txt
./non-fiction/OUP/Castro/chW.txt
./non-fiction/OUP/Castro/chM.txt
./non-fiction/OUP/Castro/chZ.txt
./non-fiction/OUP/Castro/chL.txt
./non-fiction/OUP/Castro/chN.txt
./non-fiction/OUP/Castro/chY.txt
./non-fiction/OUP/Castro/chO.txt
```

example 2: This command finds files with files that were modified less than a 21 days ago and it's useful because it helps you find all the
files modified before a certain amount of days. 

input:
```
find ./non-fiction/OUP/Berk -mtime -21
```

output:
```
./non-fiction/OUP/Berk
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Berk/ch1.txt
./non-fiction/OUP/Berk/CH4.txt
./non-fiction/OUP/Berk/ch7.txt
```
