**Compiler for Edsger Programming Language**

***written in OCaml***

**National Technical University of Athens**

**Course: Compilers**

***September 2023***

Students: Kontalexi Marina - Papadoulis George

Steps to download and run the project:  
First edit the /src/project_path.txt file and write in the first line the full path of edsger project.  
For example
```
/mnt/c/Documents/Compilers/Compilers_Edsger
```
To build the compiler run 
```bash
$ make
```
in the project directory /src.

If you want to change standard library you should add your library inside the directory src in a directory named lib
```bash
$ [project_directory]/src/lib
```

To get the project in initial state you run
```bash
$ make distclean
```

In order to run the compiler
```bash
$ ./edsger [options] [file.eds]
```
in the project directory /src.  
The given options are:
```
-O: enables compiler's optimizations and produces (a.s file)
-f: produce assembly code (a.s file)
-i: produce intermidiate code (a.ll file)

if nothing given then it produces assembly code and an executable file named a.out
```

Code Dependences:  
- llvm 18.0.0
- clang 18.0.0
- ocaml 4.14.0
- opam 2.0.5
- gcc 9.4.0
