## About
### midl - output the middle part of the file
#### Usage: midl [OPTION]

  *-n*     output the middle of K lines, instead of the middle 10;

  *-h*     display this help and exit

  In default, 10 middle lines are printed
  i.e)
```sh
    $ seq 100 | midl
    46
    47
    48
    49
    50
    51
    52
    53
    54
    55
```

  More smaller number is preferentially printed.
  * When the line number is odd and -n argument is even.
  
  i.e)
```sh
    $ seq 3 | midl -n 2
    1
    2
```

  * When the line number is even and -n argument is odd.
  
  i.e)
```sh
    $ seq 4 | midl -n 1
    2
```
