# Linux Comands

### mkdir: make directory


```
$ mkdir doc src
```

### ls: list

```
$ ls
```


```
$ ls -l
-rw-r--r-- 1 lzy lzy 8980 2月  11  2019 examples.desktop
```

- File Type: 1 bit

d: directory
-: file
l: link

- Access: 3 groups, 9 bits

3Group: user, group, others
Access: Read(r), Write(w), Exec(x), -

-a: all(noraml, hide)

```
$ ls -a
-rw-r--r-- 1 lzy lzy 8980 2月  11  2019 examples.desktop
```

### chmod

```
$ ls -l
-rw-r--r-- 1 lzy lzy 8980 2月  11  2019 examples.desktop
```

u: user
g: group
o: other

r: 4  0x0100
w: 2  0x0010
x: 1  0x0001

r:   0x0100  4
w:   0x0010  2
rw:  0x0110  6

```
$ chmod u=r examples.desktop
```

```
$ chmod u+r examples.desktop
```

```
$ chmod u-r examples.desktop
```

```
$ chmod 644 examples.desktop
```

### cd: change directory

```
$ cd ..
$ cd ~
```


### pwd: print work directory

```
$ pwd
```

### cat

```
$ cat ~/doc/linux-cookbook/linux-cmd.md
```


### which

```
$ which ls
```

### zsh

- config file:

```
$ vi ~/.zshrc
```

### GCC: GNU(Stallman)

```
$ sudo apt install build-essential
```


## GNU Make: DAG scheduler, 

Input: Makefile

define tasks and dependencies
task: (complie hello.c)
dep: no cycle, DAG

a -> b ->c->d
|           |
|------->e---

$ make -f Makefile


## vscode: editor
vs: visual studio: IDE, editor, compiler, linker, debug, ....


## c/c++

-- make

$ git clone http://github.com/google/protobuf

$ ./configure
$ make
$ sudo make install

$ ./configure

1. test os: linux, win, macos
2. test CPU
3. test pthread
...
n: generate Makefile

// Makefile
hello:
    gcc -D__GNU__ hello.c 

all: hello

$ make

$ gcc -D__GNU__ hello.c

// hello.c
#ifdef __GNU__
   int f();
#else
   int f(int);
#endif


## Build tools: DAG

c/c++: make, cmake, bazel
java: ant, maven, gradle
python: setuptools


### Compiler

c/c++: GCC(Linux), Visual Stuido(Windows), Clang on LLVM(Mac OS)
java: Oracle JDK, OpenJDK

### Editor

- vi(Bill Joy) VS. emacs(Gcc, Stallman, GNU)
- Visual Studo Code
- Sublime
- NotePad++(Windows, taiwen)

### Debug

- GDB on linux
- Visual Studio on Windows

### IDE

- Visual Studio(Windows)
- Eclipse(Linux, Windows, Mac OS)

- Python: PyCharm
- Java: Eclipse, InterllJ Idea
- Go: Goland

### PDF Viewer

```
$ sudo apt install okular
```

```
$ okular ~/Document/linux/a.pdf &
```

- father: shell
- child: okular

### Linux Basic

- Linux


### Open Source

- Docker(go)
- Kubernetes(go)
- TensorFlow(c++)
- Git(c)
