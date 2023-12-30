# C Library

## C Standard Library
- [C standard library @ wiki](https://en.wikipedia.org/wiki/C_standard_library)
- [Comparison of C/POSIX standard library implementations for Linux](http://www.etalabs.net/compare_libcs.html)
> The table below and notes which follow are a comparison of some of the different standard library implementations available for Linux, with a particular focus on the balance between feature-richness and bloat. I have tried to be fair and objective, but as I am the author of musl, that may have influenced my choice of which aspects to compare.

### ISO C
- [ISO C Names and corresponding headers](http://www.schweikhardt.net/identifiers.html#isoc)

### POSIX C
- [C POSIX library @ wiki](https://en.wikipedia.org/wiki/C_POSIX_library)
  > The C POSIX library is a specification of a C standard library for POSIX systems. It was developed at the same time as the ANSI C standard. Some effort was made to make POSIX compatible with standard C; POSIX includes additional functions to those introduced in standard C.
- [POSIX names and corresponding headers](http://www.schweikhardt.net/identifiers.html#posix)

### BSD C
- [BSD libc @ wiki](https://en.wikipedia.org/wiki/C_standard_library#BSD_libc)
> BSD libc is a superset of the POSIX standard library supported by the C libraries included with BSD operating systems such as FreeBSD, NetBSD, OpenBSD and macOS. BSD libc has some extensions that are not defined in the original standard, many of which first appeared in 1994's 4.4BSD release (the first to be largely developed after the first standard was issued in 1989). Some of the extensions of BSD libc are:
  - sys/tree.h – contains an implementation of red–black tree and splay tree[17][18]
  - sys/queue.h – implementations of Linked list, queues, tail queue, etc.[19][20]
  - fts.h – contains some functions to traverse a file hierarchy[24][25]
  - db.h – some functions to connect to the Berkeley DB[26][27]

### GNU C (Relations with the above three???)
- [The GNU C Library](https://www.gnu.org/software/libc/)
  - [The GNU C Library (glibc)](https://sourceware.org/glibc/)
  > The GNU C Library project provides the core libraries for the GNU system and GNU/Linux systems, as well as many other systems that use Linux as the kernel. These libraries provide critical APIs including ISO C11, POSIX.1-2008, BSD, OS-specific APIs and more. These APIs include such foundational facilities as open, read, write, malloc, printf, getaddrinfo, dlopen, pthread_create, crypt, login, exit and more. The GNU C Library is designed to be a backwards compatible, portable, and high performance ISO C library. It aims to follow all relevant standards including ISO C11, POSIX.1-2008, and IEEE 754-2008.
	- [The GNU C Library (glibc) manual](https://sourceware.org/glibc/manual/)

### Bionic
- [Bionic @ wiki](https://en.wikipedia.org/wiki/Bionic_%28software%29)
> Bionic is an implementation of the standard C library, developed by Google for its Android operating system.[2] It differs from the GNU C Library (glibc) in being designed for devices with less memory and processor power than a typical Linux system.
> Bionic is a C library for use with the Linux kernel, and provides libc, libdl, and libm (libpthread functionality is part of libc, not a separate library as on some other systems).
- [android / platform / bionic](https://android.googlesource.com/platform/bionic/)
  > bionic is Android's C library, math library, and dynamic linker.

### dietlibc
- [dietlibc @ wiki](https://en.wikipedia.org/wiki/Dietlibc)
> dietlibc is a C standard library released under the GNU General Public License Version 2, and proprietary licenses are also available. It was developed with the help of about 100 volunteers by Felix von Leitner with the goal to compile and link programs to the smallest possible size.[1] dietlibc was developed from scratch and thus only implements the most important and commonly used functions. It is mainly used in embedded devices.
- [diet libc - a libc optimized for small size](https://www.fefe.de/dietlibc/)

### uClibc
- [uClibc @ wiki](https://en.wikipedia.org/wiki/UClibc)
> In computing, uClibc (sometimes written µClibc) is a small C standard library intended for Linux kernel-based operating systems for embedded systems and mobile devices. uClibc was written to support μClinux, a version of Linux not requiring a memory management unit and thus suited for microcontrollers (uCs; the "u" is a Latin script typographical approximation - not a proper romanization, which would be letter "m" - of μ for "micro").
- [uClibc](https://www.uclibc.org/)
- [uClibc-ng - Embedded C library](https://uclibc-ng.org/)
  > uClibc-ng is a small C library for developing embedded Linux systems. It is much smaller than the GNU C Library, but nearly all applications supported by glibc also work perfectly with uClibc-ng.
### musl
- [musl @ wiki](https://en.wikipedia.org/wiki/Musl)
> musl is a C standard library intended for operating systems based on the Linux kernel, released under the MIT License.[3] It was developed by Rich Felker with the goal to write a clean, efficient, and standards-conformant libc implementation.
- [musl libc](https://musl.libc.org/)
> musl is an implementation of the C standard library built on top of the Linux system call API, including interfaces defined in the base language standard, POSIX, and widely agreed-upon extensions. musl is lightweight, fast, simple, free, and strives to be correct in the sense of standards-conformance and safety.
### Toybox
- [Toybox @ wiki](https://en.wikipedia.org/wiki/Toybox)
> Toybox is a free and open-source software implementation of over 200 Unix command line utilities such as ls, cp, and mv. The Toybox project was started in 2006,[3] and became a 0BSD licensed BusyBox alternative.[4][5] Toybox is used for most of Android's command-line tools in all currently supported Android versions, and is also used to build Android on Linux and macOS. All of the tools are tested on Linux, and many of them also work on BSD and macOS.
- [toybox](http://www.landley.net/toybox/)
> Toybox combines many common Linux command line utilities together into a single BSD-licensed executable. It's simple, small, fast, and reasonably standards-compliant (POSIX-2008 and LSB 4.1).

- [/NetBSD/lib/libc/](http://bxr.su/NetBSD/lib/libc/)

- [/FreeBSD/lib/libc/](http://bxr.su/FreeBSD/lib/libc/)

- [/OpenBSD/lib/libc/](http://bxr.su/OpenBSD/lib/libc/)

- [/DragonFly/lib/libc/](http://bxr.su/DragonFly/lib/libc/)

## Extensions
- [awesome-c @ github](https://github.com/oz123/awesome-c)
> A curated list of awesome C frameworks, libraries, resources and other shiny things. Inspired by all the other awesome-... projects out there.

- [tbox @ github](https://github.com/tboox/tbox/tree/master)
> TBOX is a glib-like cross-platform C library that is simple to use yet powerful in nature.

> The project focuses on making C development easier and provides many modules (.e.g stream, coroutine, regex, container, algorithm ...), so that any developer can quickly pick it up and enjoy the productivity boost when developing in C language.

> It supports the following platforms: Windows, Macosx, Linux, Android, iOS, *BSD and etc.

- [mlib @ github](https://github.com/P-p-H-d/mlib)
> Library of generic and type safe containers in pure C language (C99 or C11) for a wide collection of container (comparable to the C++ STL).

- [Gena @ github](https://github.com/cher-nov/Gena)
> Generic pseudo-templated containers for C. Written entirely in C89 with design inspired by the C++ STL. /// DOCS ARE SLIGHTLY OUTDATED, PROJECT IS STABLE AND STILL BEING DEVELOPED

- [nuklear @ github](https://github.com/golang-ui/nuklear)
> This project provides Go bindings for nuklear.h — a small ANSI C GUI library.