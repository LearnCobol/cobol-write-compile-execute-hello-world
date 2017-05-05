# cobol-write-compile-execute-hello-world
Cobol Hello World: Write, Compile and Execute Cobol on Linux OS

1. Write the Hello World Cobol Program

  Create helloworld.cbl program using your favorite editor.

2. Make sure Cobol Compiler is installed on your system

  $ whereis cobc
  cobc: /usr/bin/cobc /usr/share/man/man1/cobc.1.gz

  $ which cobc
  /usr/bin/cobc

3. Installing cobc compiler

If you don’t have cobol compiler, install it as shown below.

  $ sudo apt-get install open-cobol

3. Compile the cobol program

Compile the HelloWorld which will create the HelloWorld executable.

  $ cobc -free -x -o helloworld-exe helloworld

  $ ls
  
  helloworld  helloworld-exe*

-free – use free source format. Without this option cobol program requires certain format.
-x – build executable program.
-o FILE – place the output file into the specified FILE.

4. Execute the cobol Program

Execute by mentioning the program name.

  $./helloworld-exe
  Hello World!
