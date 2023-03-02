# minitalk

Project instructions
• Name your executable files client and server.
• You have to turn in a Makefile which will compile your source files. It must not
relink.
• You can definitely use your libft.
• You have to handle errors thoroughly. In no way your program should quit unex-
pectedly (segmentation fault, bus error, double free, and so forth).
• Your program mustn’t have memory leaks.
• You can have one global variable per program (one for the client and one for
the server), but you will have to justify their use.
• In order to complete the mandatory part, you are allowed to use the following
functions:
◦ write
◦ ft_printf and any equivalent YOU coded
◦ signal
◦ sigemptyset
◦ sigaddset
◦ sigaction
◦ kill
◦ getpid
◦ malloc
◦ free
◦ pause
◦ sleep
◦ usleep
◦ exit

You must create a communication program in the form of a client and a server.
• The server must be started first. After its launch, it has to print its PID.
• The client takes two parameters:
◦ The server PID.
◦ The string to send.
• The client must send the string passed as a parameter to the server.
Once the string has been received, the server must print it.
• The server has to display the string pretty quickly. Quickly means that if you think
it takes too long, then it is probably too long.
• Your server should be able to receive strings from several clients in a row without
needing to restart.
• The communication between your client and your server has to be done only using
UNIX signals.
• You can only use these two signals: SIGUSR1 and SIGUSR2

Bonus part
Bonus list:
• The server acknowledges every message received by sending back a signal to the
client.
• Unicode characters support!
