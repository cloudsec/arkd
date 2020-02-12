# arkd
The kernel debugger script for checking kernel level rootkits.
by wzt 2020	http://github.com/cloudsec

All the structure offset is hardcoded base on:
win10-1903 amd64, kernel version 18362

0: kd> $$>a<d:\wzt\nt\arkd\arkd.txt 0
Anti Rootkit - The Kernel Debugger Scripts v0.01.
by wzt  http://github.com/cloudsec
usage: <options>
options:
0       --      show the commond list.
1       --      check hidden process.
2       --      check hidden driver.
3       --      list PspcidTable.
4       --      list process create callback notify routine.
5       --      list thread create callback notify routine.
6       --      list driver create callback notify routine.
7       --      list ssdt.
8       --      list ssdt hook.
9       --      check ssdt/ssdt_shadow inline hook.
10      --      list process vads.
