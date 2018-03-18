---
layout: post
title: Setup Golang on Fedora 27!
categories: golang
---

### This blog going to setup Golang tool step by step;


>    Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.

<!--more-->
    
>    Go is expressive, concise, clean, and efficient. Its concurrency mechanisms make it easy to write programs that get the most out of multicore and networked machines, while its novel type system enables flexible and modular program construction. Go compiles quickly to machine code yet has the convenience of garbage collection and the power of run-time reflection. It’s a fast, statically typed, compiled language that feels like a dynamically typed, interpreted language.

Why Go:
----------------------

Go is clean and simple. Main fetures Go has goroutines. Goroutines simillar to threads but it more efficient. Consume less memory from the heap and lighter than threads.


Intalling Go tools:
----------------------

* First option to installing the Go from your distrobution package where I'm going to use RPM based.

* Second option is from GO binary https://golang.org/dl/.

**From distro package:**

```
$ sudo dnf install golang
```
    
**From Binary:**

> Download the archive and extract it into /usr/local, creating a Go tree in /usr/local/go

```
$ wget https://dl.google.com/go/go$VERSION.$OS-$ARCH.tar.gz
```

> Add /usr/local/go/bin to the PATH environment variable into /etc/profile or $HOME/.bashrc

```
export PATH=$PATH:/usr/local/go/bin
```

> Go code setup workspace which is defined by the GOPATH environment variable.
> Default it set to $HOME/go

```
$ mkdir -p $HOME/go
$ go env GOPATH
```

> Change it by adding new path into $HOME/.bashrc
```
$ echo 'export GOPATH=$HOME/new/go' >> $HOME/.bashrc
```


Reference
----------
* [Golang Home Page](https://golang.org/)

