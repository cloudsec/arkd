# arkd
The kernel debugger script for checking kernel level rootkits.

- by wzt 2020	(http://github.com/cloudsec)
- All the structure offset is hardcoded base on:
- win10-1903 amd64, kernel version 18362

# usage
```
0: kd> $$>a<d:\wzt\nt\arkd\arkd.txt 0
The Kernel Debugger Scripts for checking rootkits v0.08.
Copyright (c) wzt 2020  http://github.com/cloudsec

usage: <options>
options:
0               --      show the commond list.
1 <0/1>         --      check hidden process.
                        0 - normal check | 1 - deep check.
2               --      check hidden driver.
3               --      list PspcidTable.
4               --      list process create callback notify routine.
5               --      list thread create callback notify routine.
6               --      list driver create callback notify routine.
7               --      list ssdt.
8               --      list ssdt hook.
9               --      check ssdt/ssdt_shadow inline hook.
10 <pid>        --      list process vads.
11              --      check object hook.
12              --      list security descriptor.
13 <pid>        --      privilege escalation of the process.
```
