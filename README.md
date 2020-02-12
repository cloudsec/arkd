# arkd
The kernel debugger script for checking kernel level rootkits.

$$ The kernel debugger script for checking kernel level rootkits.

$$ by wzt 2020	http://github.com/cloudsec

$$

$$ All the structure offset is hardcoded base on:

$$ win10-1903 amd64, kernel version 18362

$$

.if (${$arg1} == 0)
{
	.printf "Anti Rootkit - The Kernel Debugger Scripts v0.01.\n"
	.printf "by wzt\thttp://github.com/cloudsec\n\n"
	.printf "usage: <options>\n"
	.printf "options:\n"
	.printf "0\t--\tshow the commond list.\n"
	.printf "1\t--\tcheck hidden process.\n"
	.printf "2\t--\tcheck hidden driver.\n"
	.printf "3\t--\tlist PspcidTable.\n"
	.printf "4\t--\tlist process create callback notify routine.\n"
	.printf "5\t--\tlist thread create callback notify routine.\n"
	.printf "6\t--\tlist driver create callback notify routine.\n"
	.printf "7\t--\tlist ssdt.\n"
	.printf "8\t--\tlist ssdt hook.\n"
	.printf "9\t--\tcheck ssdt/ssdt_shadow inline hook.\n"
	.printf "10\t--\tlist process vads.\n"
}
