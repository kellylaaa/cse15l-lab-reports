# Lab Report 3

## Researching Commands
1. `find -name`

example 1: This command is useful because it helps find the file with the name "ch.1"

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

example 2: This command is useful because it helps find the file with the name "ch.2"

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

2. `find -type`
example 1:

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

example 2:

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

3. `find -size`

example 1:                                                         
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

example 2:                                                         
input: 
```
find ./non-fiction/OUP/Berk -size +100k
```

output:
```
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Berk/CH4.txt
```
