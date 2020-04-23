# Hello, World!

Filename: hello.cpc
```cpc
txt/ Hello, world!
```
Listing 1-1: A program that prints `Hello, world!`

Save the file and go back to your terminal window. On **GNU**/Linux, enter the following commands to compile and run the file:
```text
$ cpcsc hello.cpc
$ ld -o hello hello.o -lcpc_runtime
$ ./hello
Hello, world!
```

On Windows, enter the following commands:
```powershell
> cpcsc hello.cpc
> cl hello.o libcpc_runtime.lib /link /out:hello.exe
> .\hello.exe
Hello, world!
```