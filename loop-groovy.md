## Groovy Loops

### upto keyword
Print number from 0 to 10 using groovy
```console
1.upto(10) {println "$it"}
```
upto keyword is used to print number from 1 to 10 here

#### Outupt:
```console
pankaj@pankajv:~/Downloads$ groovy loop.groovy 
1
2
3
4
5
6
7
8
9
10
```
### times keyword
```cosnole
10.times{println "$it"}
```
#### Output
```console
pankaj@pankajv:~/Downloads$ groovy times.groovy 
0
1
2
3
4
5
6
7
8
9
```

### step keyword
```console
0.step(9,2){println "$it"}
```
#### Output
```console
pankaj@pankajv:~/Downloads$ groovy step.groovy 
0
2
4
6
8
```
