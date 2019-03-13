# Awesome C #

A curated list of C good stuff.

**An important note:** first and foremost linked resources are for C, therefore
C++ is an afterthought.

**Note:** there are several awesome-c lists already, but they are having
somewhat different sets of libraries in them. This list tries to incorporate
them all, and many more other resources. Consider it my personal cheat sheet and
index for easier search instead of github stars. Also, original list categories
are a mess.

Incorporated lists:

* https://github.com/aleksandar-todorovic/awesome-c (rare updates, too vague and
  sometimes mismatched categories, not very wide selection of content)
* https://github.com/kozross/awesome-c (updated regularly, but has even less
  content than one above)
* https://github.com/uhub/awesome-c (regular updated, much more content, but
  much more of it doesn't even belong to C list. Also, no structure at all)

--------------------------------------------------------------------------------

## Index ##

* [Meta](#meta)
	* [Standarts](#standarts)
	* [Tooling](#tooling)
		* [Build Systems](#build-systems)
		* [Compilers](#compilers)
		* [Debugging and Analysis](#debugging-and-analysis)
		* [Documentation Generation](#documentation-generation)
		* [Editors](#editors)
		* [Microsoft Windows Environment](#microsoft-windows-environment)
		* [Profiling](#profiling)
		* [Text Editor Extensions](#text-editor-extensions)
		* [Utilities](#utilities)
	* [Reading material](#reading-material)
		* [Books](#books)
			* [Reference Books](#reference-books)
			* [Beginner Books](#beginner-books)
			* [Intermediate Books](#intermediate-books)
			* [Advanced Books](#advanced-books)
		* [Articles and Other Resources](#articles-and-other-resources)
			* [Reference](#reference)
			* [Benchmarks](#benchmarks)
			* [Beginner Level](#beginner-level)
			* [Intermediate Level](#intermediate-level)
			* [Advanced Level](#advanced-level)
		* [Code Examples](#code-examples)
		* [Courses](#courses)

--------------------------------------------------------------------------------

* [AI](#ai)
* [Algoritm Implementations](#algoritm-implementations)
* [Argument Parsing](#argument-parsing)
* [Calculations](#calculations)
* [Compression](#compression)
* [Concurrency and Parallelism](#concurrency-and-parallelism)
* [Crypto](#crypto)
* [Databases](#databases)
* [Data Structures](#data-structures)
* [Events](#events)
* [FFI](#ffi)
* [Flow Control and Language Extension](#flow-control-and-language-extension)
* [Game Development](#game-development)
* [Graphics](#graphics)
* [GUI](#gui)
* [Hardware Oriented](#hardware-oriented)
* [Hashing](#hashing)
* [Image Processing and Computer Vision](#image-processing-and-computer-vision)
* [Integrated Debugging](#integrated-debugging)
* [Lexing and Parsing](#lexing-and-parsing)
* [Memory Management](#memory-management)
* [Multimedia](#multimedia)
* [Multiple Purpose Libraries](#multiple-purpose-libraries)
* [Networking](#networking)
	* [DNS](#dns)
	* [HTTP](#http)
	* [Mail](#mail)
	* [Messaging](#messaging)
	* [Other Networking](#other-networking)
	* [Websockets](#websockets)
* [OS Specifics](#os-specifics)
* [Procedural Generation](#procedural-generation)
* [Regex](#regex)
* [Serialization](#serialization)
* [Source Code Collections](#source-code-collections)
* [Standard Libraries](#standart-libraries)
* [String Manipulation](#string-manipulation)
* [Structured File Processing](#structured-file-processing)
	* [Binaries](#binaries)
	* [CSV](#csv)
	* [JSON](#json)
	* [INI](#ini)
	* [Other Filetypes](#other-filetypes)
	* [XML](#xml)
	* [YAML](#yaml)
* [Testing](#testing)
* [TUI](#tui)
* [Web Frameworks](#web-frameworks)
* [Web Service APIs](#web-service-apis)

--------------------------------------------------------------------------------

* [Uncategorized](#uncategorized)
* [Unsorted](#unsorted)

--------------------------------------------------------------------------------

## Meta ##
### Standarts ###
<details>
  <summary>Click to expand</summary>

  * [Draft C89 standard][1-1]
  * [Draft C99 standard][1-2]
  * [Draft C11 standard][1-3]
  * [Draft C18 standard][1-4]

  [1-1]: https://port70.net/~nsz/c/c89/c89-draft.html
  [1-2]: https://port70.net/~nsz/c/c99/n1256.html
  [1-3]: https://port70.net/~nsz/c/c11/n1570.html
  [1-4]: https://web.archive.org/web/20181230041359if_/http://www.open-std.org/jtc1/sc22/wg14/www/abq/c17_updated_proposed_fdis.pdf
</details>

### Tooling ###
#### Build Systems ####
* [aimake][2-1] - Build tool designed to avoid complex configurations. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Autoconf][2-2] - Extensible package of M4 macros that produce shell scripts
  to automatically configure software source code packages. Part of the
  Autotools. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Automake][2-3] - Tool for automatically generating `Makefile.in` files
  compliant with the GNU Coding Standards. Requires the use of Autoconf. Part of
  the Autotools. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Bazel][2-4] - Build system for various operating systems and targets. [``Apache-2.0``][Apache-2.0]
* [Buck][2-5] - Build system created and used by Facebook. [``Apache-2.0``][Apache-2.0]
* [CMake][2-6] - Cross-platform family of tools designed to build, package and
  test software. Written in C++11. [``BSD-3-Clause``][BSD-3-Clause]
* [GNU Make][2-7] - Tool which controls the generation of executables and other
  non-source files of a program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GMSL][2-8] - GNU Make Standard Library; a collection of additional
  functionality for GNU Make. [``BSD-3-Clause``][BSD-3-Clause]
* [Jam][2-9] - Build system, designed to be easier than make. Understands C
  build rules implicitly. [``Jam License``][2-10]
* [Libtool][2-11] - Generic library support script. Part of the Autotools. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Meson][2-12] - Build system based on Ninja and Python. [``Apache-2.0``][Apache-2.0]
* [Ninja][2-13] - Small, simple build system with a focus on speed. [``Apache-2.0``][Apache-2.0]
* [Premake][2-14] - Generates project files for Visual Studio, Xcode and GNU
  Make. Targets suppport can be extended via modules. [``BSD-3-Clause``][BSD-3-Clause]
* [Qbs][2-15] - Modern build tool for software projects. [``LGPL-3.0-only``][LGPL-3.0-only]
* [qmake][2-16] - Build system included with the Qt Framework. [`GNU GPL3 with Qt Exception`][2-17]
* [SCons][2-18] - Software construction tool based on Python. [``MIT``][MIT]
* [xmake][2-19] - Cross-platform build utility based on Lua. [``Apache-2.0``][Apache-2.0]
* [zproject][2-20] - Project generator and build system support tool for ZeroMQ
  project. [``MPL-2.0``][MPL-2.0]
* [tup](http://gittup.org/tup/index.html) - Very fast, file-based, cross-platform build system. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [gittup/tup](https://github.com/gittup/tup) - Tup is a file-based build system.
* [jamplus/jamplus](https://github.com/jamplus/jamplus) - Jamplus is a generic code and data build system derived from the original Perforce version of Jam

[2-1]: http://nethack4.org/projects/aimake/
[2-2]: https://www.gnu.org/software/autoconf/autoconf.html
[2-3]: https://www.gnu.org/software/automake/automake.html
[2-4]: https://bazel.build/
[2-5]: https://buckbuild.com/
[2-6]: https://cmake.org/
[2-7]: https://www.gnu.org/software/make/
[2-8]: https://gmsl.sourceforge.net/
[2-9]: https://www.perforce.com/documentation/jam-documentation
[2-10]: https://en.wikipedia.org/wiki/Perforce_Jam#License
[2-11]: https://www.gnu.org/software/libtool/
[2-12]: http://mesonbuild.com/
[2-13]: https://github.com/ninja-build/ninja
[2-14]: https://github.com/premake/premake-core
[2-15]: http://doc.qt.io/qbs/
[2-16]: https://doc.qt.io/qt-5/qmake-manual.html
[2-17]: https://github.com/qt/qtbase/blob/5.11/LICENSE.GPL3-EXCEPT
[2-18]: https://www.scons.org/
[2-19]: https://xmake.io/
[2-20]: https://github.com/zeromq/zproject

#### Compilers ####
* [Clang][3-2] - Compiler for LLVM. Supports C11. [``NCSA``][NCSA]
* [CompCert][3-5] - Fully-verified C compiler. Supports almost all of C89. [`GPL2.1-or-later`][GPL-2.0-or-later]
* [GCC][3-1] a C compiler as part of its compiler set. Supports C11. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Intel SPMD][3-7] - Compiler for a variant of the C language, for single
  program, multiple data programming. [``Various licenses``][3-8]
* [PCC][3-3] - Venerable compiler. Supports C99. [``Various licenses``][3-4]
* [TCC][3-6] - Tiny C Compiler; a small, fast C compiler. Supports C99 (except
  complex types). [``LGPL2.1``][LGPL-2.1-only]
* [rui314/8cc](https://github.com/rui314/8cc) - A Small C Compiler
* [LuaDist/tcc](https://github.com/LuaDist/tcc) - Small but fast C compiler.  Supports ANSI C, most of the new ISO C99 standard, and many GNUC extensions, including inline assembly.
* [TinyCC/tinycc](https://github.com/TinyCC/tinycc) - Mirror from mob branch
* [alexfru/SmallerC](https://github.com/alexfru/SmallerC) - Simple C compiler
* [andrewchambers/c](https://github.com/andrewchambers/c) - small self hosting C compiler
* [cc65/cc65](https://github.com/cc65/cc65) - cc65 - a freeware C compiler for 6502 based systems —
* [drh/lcc](https://github.com/drh/lcc) - The lcc retargetable ANSI C compiler
* [jserv/amacc](https://github.com/jserv/amacc) - Small C Compiler generating ELF executable for Arm architecture
* [larmel/lacc](https://github.com/larmel/lacc) - A simple, self-hosting C compiler

[3-1]: https://gcc.gnu.org/
[3-2]: https://clang.llvm.org/
[3-3]: http://pcc.ludd.ltu.se/
[3-4]: http://pcc.ludd.ltu.se/licenses/
[3-5]: http://compcert.inria.fr/
[3-6]: https://bellard.org/tcc/
[3-7]: http://ispc.github.io/
[3-8]: https://github.com/ispc/ispc/blob/master/LICENSE.txt

#### Debugging and Analysis ####
* [address-sanitizer][4-3] - Fast memory error detector. [``Apache-2.0``][Apache-2.0]
* [C-Reduce][4-1] - Tool that takes a large C file with a property of interest
  and automatically produces a much smaller C file that has the same property.
  Intended to help create minimal bug-demonstrating cases in complex code. [``BSD-3-Clause``][BSD-3-Clause]
* [CBMC][4-2] - C Bounded Model Checker; a tool for verification of array
  bounds, pointer safety and user-specified assertions. [``BSD-4-Clause``][BSD-4-Clause]
* [ClangCheck][4-4] - Static analysis tool, designed to work with Clang. [``NCSA``][NCSA]
* [Cppcheck][4-5] - Static analysis tool. Despite the name, works well with C. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GNU cflow][4-6] - Analyzes a collection of source files and prints a graph
  charting control flow in the program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GNU Complexity][4-7] - Tool for measuring the complexity of source code. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [CScout][4-8] - Source code analyzer and refactoring browser for C programs. [``GPL-3.0-only``][GPL-3.0-only]
* [GNU DDD][4-9] - Graphical front-end for a range of command-line debuggers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GDB][4-10] - GNU Project debugger. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [lldb][4-11] - LLVM debugger. [``NCSA``][NCSA]
* [rr][4-12] - Debugger that records non-deterministic executions to allow for
  deterministic debugging. [``BSD-2-Clause``][BSD-2-Clause]
* [Valgrind][4-13] - Range of dynamic analysis tools, including a leak checker. [``GPL-2.0-only``][GPL-2.0-only]
* [SVF-tools/SVF](https://github.com/SVF-tools/SVF) - Pointer Analysis and Program Dependence Analysis for C and C++ Programs
* [agl/ctgrind](https://github.com/agl/ctgrind) - Checking that functions are constant time with Valgrind
* [cgdb/cgdb](https://github.com/cgdb/cgdb) - Console front-end to the GNU debugger

[4-1]: https://embed.cs.utah.edu/creduce/
[4-2]: https://www.cprover.org/cbmc/
[4-3]: https://github.com/google/sanitizers
[4-4]: https://clang.llvm.org/docs/ClangCheck.html
[4-5]: http://cppcheck.sourceforge.net/
[4-6]: http://www.gnu.org/software/cflow/
[4-7]: https://www.gnu.org/software/complexity/
[4-8]: https://www.spinellis.gr/cscout/
[4-9]: https://www.gnu.org/software/ddd/ddd.html
[4-10]: https://www.gnu.org/software/gdb/
[4-11]: https://lldb.llvm.org/
[4-12]: https://rr-project.org/
[4-13]: http://www.valgrind.org/

#### Documentation Generation ####
* [Cxref][5-1] - Generates documentation in either LaTeX, HTML, RTF or SGML. [``GPL-2.0-only``][GPL-2.0-only]
* [DocOnce][5-2] - Modestly tagged markup language that can be used to generate
  a range of formats. [``BSD-3-Clause``][BSD-3-Clause]
* [Doxygen][5-3] - De-facto standard tool for generating documentation from
  annotated sources. Can generate a large range of formats. [``GPL-2.0-only``][GPL-2.0-only]
* [GTK-Doc][5-4] - Tool for generating C documentation from annotated sources.
  Has support for the Autotools. Various licenses.

[5-1]: http://www.gedanken.org.uk/software/cxref/
[5-2]: https://hplgit.github.io/doconce/doc/web/index.html
[5-3]: http://www.doxygen.nl/
[5-4]: https://www.gtk.org/gtk-doc/

#### Editors ####
* [Anjuta DevStudio][6-1] - GNOME IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Atom][6-3] - Hackable text editor for the 21st century. [``MIT``][MIT]
* [Code::Blocks][6-2] - Extendable, configurable IDE supporting C. [``GPL-3.0-only``][GPL-3.0-only]
* [CodeLite][6-4] - Cross-platform IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Eclipse][6-6] - IDE written in Java. [``EPL``][6-7]
* [Geany][6-5] - Small and fast IDE. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [KDevelop][6-8] - KDE IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Qt Creator][6-9] - Cross-platform IDE written with C++ and Qt, part of the
  Qt SDK. Supports Clang Code Model. [``GNU GPL3 with Qt exception``][6-10]
* [Visual Studio Code][6-11] - Code editing, redefined. Visual Studio Code. [``MIT``][MIT]

[6-1]: http://anjuta.org/
[6-2]: http://www.codeblocks.org/
[6-3]: https://atom.io/
[6-4]: https://codelite.org/
[6-5]: https://www.geany.org/
[6-6]: http://www.eclipse.org/ide/
[6-7]: https://directory.fsf.org/wiki/License:EPL-1.0
[6-8]: https://www.kdevelop.org/
[6-9]: https://www.qt.io/qt-features-libraries-apis-tools-and-ide/#ide
[6-10]: https://github.com/qt-creator/qt-creator/blob/master/LICENSE.GPL3-EXCEPT
[6-11]: https://github.com/Microsoft/vscode

#### Microsoft Windows Environment ####
* [Cygwin][7-1] - Designed to emulate a POSIX-compatible environment extensively
  under Windows. [Various licenses, all open source][7-2].
* [MinGW-w64][7-3] - Minimalist environment for C development on Windows with
  64 bit support. [Various licenses, all open source][7-4].
* [MSYS2][7-5] - Minimal SYStem 2; aims to provide support for a POSIX
  environment on Windows, with a package manager based on Arch Linux's
  pacman. Packages have individual licenses, otherwise, as MinGW and Cygwin.
* [reactos/reactos](https://github.com/reactos/reactos) - A free Windows-compatible Operating System

[7-1]: https://cygwin.com/
[7-2]: https://cygwin.com/licensing.html
[7-3]: http://mingw-w64.yaxm.org/doku.php/start
[7-4]: http://mingw.org/license
[7-5]: http://msys2.github.io/

#### Profiling ####
* [gperftools][8-1] - Collection of utilities for measuring and improving
  performance. [``BSD-3-Clause``][BSD-3-Clause]
* [gprof][8-2] - Performance analysis tool. Part of GNU binutils. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [OProfile][8-3] - Statistical profiler for Linux. Can profile any code
  (including the kernel!) with low overhead and without recompilation. [``GPL-2.0-only``][GPL-2.0-only]
* [perf][8-4] - Linux kernel-based profiler with a lot of functionality. [``GPL-2.0-only``][GPL-2.0-only]

[8-1]: https://github.com/gperftools/gperftools
[8-2]: https://www.gnu.org/software/binutils/
[8-3]: http://oprofile.sourceforge.net/news/
[8-4]: https://perf.wiki.kernel.org/index.php/Main_Page

#### Text Editor Extensions ####
* [CCompletion][9-1] - Notepad++ autocompletion plugin. Works with all
  identifiers recognized by Ctags. This is a download link. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [CEDET][9-2] - Collection of Emacs Development Environment Tools; designed to
  provide IDE-like features to Emacs. Built-in. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Flycheck][9-3] - Modern syntax checking for Emacs. For C, it can use either
  GCC or Clang as a back-end. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [linter-clang][9-4] - Lint C code in Atom, using Clang. [``MIT``][MIT]
* [linter-gcc][9-5] - Lint C code in Atom, using GCC. [``MIT``][MIT]
* [Neomake][9-6] - Async :make and linting framework for Neovim/Vim. [``MIT``][MIT]
* [Syntastic][9-7] - Syntax checking and linting for Vim. [``WTFPL``][WTFPL]
* [YASnippet][9-8] - Emacs code template system, with C templates for common
  snippets. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [YouCompleteMe][9-9] - Code completion engine for Vim. [``GPL-3.0-only``][GPL-3.0-only]
* [lvzixun/Clang-Complete](https://github.com/lvzixun/Clang-Complete) - a auto complete plugin for sublimetext3

[9-1]: http://freeweb.siol.net/rmihor/NppCCompletionPlugin.zip
[9-2]: http://cedet.sourceforge.net/
[9-3]: https://github.com/flycheck/flycheck
[9-4]: https://github.com/AtomLinter/linter-clang
[9-5]: https://github.com/hebaishi/linter-gcc
[9-6]: https://github.com/neomake/neomake
[9-7]: https://github.com/vim-syntastic/syntastic
[9-8]: http://joaotavora.github.io/yasnippet/
[9-9]: http://valloric.github.io/YouCompleteMe/

#### Utilities ####
* [Artistic Style][10-4] - Fast and small automatic source code formatter that
  supports C. [``LGPL-3.0-only``][LGPL-3.0-only]
* [biicode][10-5] - Dependency manager. [``MIT``][MIT]
* [c][10-6] - Compile and execute C "scripts" in one go on the command line. Also
  has shebang support. [``MIT``][MIT]
* [c99sh][10-7] - Run C files using hash-bang. [``BSD-2-Clause``][BSD-2-Clause]
* [ccache][10-1] - Compiler cache designed to speed up recompilation. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [cdecl][10-8] - Online service to translate C declarations into English and
  vice versa. Public domain.
* [cinclude2dot][10-9] - Graphs include dependencies in a project using Graphviz. [GPL-1.0-or-later][335] or [``GPL-2.0-or-later``][GPL-2.0-or-later] or [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [distcc][10-2] - Program that allows builds to be distributed among several
  machines. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [Firm][10-3] - Library that provides a graph-based intermediate representation,
  optimizations and assembly code generation suitable for use in compilers.
  Comes with an example C front-end under the same license. [``LGPL-2.1-only``][LGPL-2.1-only]
* [GNU Global][10-10] - Source code tagging tool. [``GPL-3.0-only``][GPL-3.0-only]
* [GPP][10-11] - General-purpose preprocessor. More versatile than the C
  preprocessor, but more flexible than m4. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [Highlight][10-12] - Converts source code to formatted text with highlighting. [``GPL-3.0-only``][GPL-3.0-only]
* [include-what-you-use][10-13] - Helps find unecessary inclusions and make
  suggestions for fixing them. Based on LLVM/Clang (and only works with it). [``NCSA``][NCSA]
* [indent][10-14] - Formats C source code automatically to make it easier to
  read. Also converts from one style of source to another. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [SMACK][10-15] - Modular software verification toolchain and a self-contained
  software verifier. Currently only works with programs compiled using Clang. [``MIT``][MIT]
* [unifdef][10-16] - Removes #ifdef and #if directives with their delimited text
  without touching any other part of the file. [``BSD-3-Clause``][BSD-3-Clause] or [``BSD-2-Clause``][BSD-2-Clause]
* [mcpp](http://mcpp.sourceforge.net/) - Portable C preprocessor. [`2-clause BSD`](https://opensource.org/licenses/BSD-2-Clause)
* [Capstone](https://github.com/aquynh/capstone) - Dissasembly/disassembler framework. [`BSD 3-clause`](https://github.com/aquynh/capstone/blob/master/LICENSE.TXT)
* [anael-seghezzi/CToy](https://github.com/anael-seghezzi/CToy) - Interactive C coding environment
* [aquynh/capstone](https://github.com/aquynh/capstone) - Capstone disassembly/disassembler framework: Core (Arm, Arm64, BPF, EVM, M68K, M680X, MOS65xx, Mips, PPC, Sparc, SystemZ, TMS320C64x, Web Assembly, X86, X86_64, XCore) + bindings.
* [buserror/simavr](https://github.com/buserror/simavr) - simavr is a lean, mean and hackable AVR simulator for linux & OSX
* [ggreer/the_silver_searcher](https://github.com/ggreer/the_silver_searcher) - A code-searching tool similar to ack, but faster.
* [jacob-carlborg/dstep](https://github.com/jacob-carlborg/dstep) - A tool for converting C and Objective-C headers to D modules
* [jbremer/darm](https://github.com/jbremer/darm) - A light-weight and efficient disassembler written in C for the ARMv7 instruction set.
* [jimenezrick/patch-AuthenticAMD](https://github.com/jimenezrick/patch-AuthenticAMD) - Utility to patch binaries generated by the Intel C++ Compiler to get the maximum performance on AMD CPUs
* [libav/c99-to-c89](https://github.com/libav/c99-to-c89) - Tool to convert C99 code to MSVC-compatible C89
* [m-schmoock/lcpp](https://github.com/m-schmoock/lcpp) - A Lua C PreProcessor

[10-1]: https://ccache.samba.org/
[10-2]: https://github.com/distcc/distcc
[10-3]: https://pp.ipd.kit.edu/firm/
[10-4]: http://astyle.sourceforge.net/
[10-5]: https://biicode.github.io/biicode/
[10-6]: https://github.com/ryanmjacobs/c
[10-7]: https://github.com/RhysU/c99sh
[10-8]: https://cdecl.org/
[10-9]: https://www.flourish.org/cinclude2dot/
[10-10]: https://www.gnu.org/software/global/
[10-11]: https://logological.org/gpp
[10-12]: http://www.andre-simon.de/doku/highlight/en/highlight.php
[10-13]: https://github.com/include-what-you-use/include-what-you-use
[10-14]: https://www.gnu.org/software/indent/
[10-15]: https://github.com/smackers/smack
[10-16]: http://dotat.at/prog/unifdef/

### Reading Material ###
#### Books ####
##### Reference Books #####
* [C in a Nushell 2E][11-1] - Concise reference book for C11.
* [C Pocket Reference][11-2] - Concise reference book for C99.
* [C: A Reference Manual 5E][11-3] - Full reference book for C99.
* [SEI CERT C Coding Standard][11-4] - Coding  recommendations from CERT.
* [The C Programming Language 2E][11-5] - Original book on C, by its creators.

[11-1]: http://shop.oreilly.com/product/0636920033844.do
[11-2]: http://shop.oreilly.com/product/9780596004361.do
[11-3]: http://careferencemanual.com/
[11-4]: https://wiki.sei.cmu.edu/confluence/display/c/SEI+CERT+C+Coding+Standard
[11-5]: https://en.wikipedia.org/wiki/The_C_Programming_Language

##### Beginner Books #####
* [C Primer Plus 6E][12-1] - Complete tutorial on programming in C11.
* [C Programming: A Modern Approach][12-2] - Book to learn the basics of C.
* [Head First C][12-3] - 'Head-first' style book for learning C.
* [The GNU C Programming Tutorial][12-4] - Beware, GNU C is not standart C.
* [careermonk/DataStructuresAndAlgorithmsMadeEasy](https://github.com/careermonk/DataStructuresAndAlgorithmsMadeEasy) - Data Structures And Algorithms Made Easy

[12-1]: https://www.pearson.com/us/higher-education/program/Prata-C-Primer-Plus-6th-Edition/PGM4399.html
[12-2]: http://knking.com/books/c2/index.html
[12-3]: http://shop.oreilly.com/product/0636920015482.do
[12-4]: http://www.crasseux.com/books/ctut.pdf

##### Intermediate Books #####
* [21st Century C][13-1] - Programming book on C that touches tooling subject.
* [Understanding and Using C Pointers][13-2] - In-depth book on pointers in C.

[13-1]: http://shop.oreilly.com/product/0636920033677.do
[13-2]: http://shop.oreilly.com/product/0636920028000.do

##### Advanced Books #####
* [Expert C Programming: Deep C Secrets][14-1] - Interesting, in-depth and
  entertaining look at the innards of C.
* [C Programming Wikibook][14-2] - Actually touches topics for all levels.

[14-1]: https://dl.acm.org/citation.cfm?id=179241
[14-2]: https://en.wikibooks.org/wiki/C_Programming

#### Articles and Other Resources ####
##### Reference #####
* [C FAQ - comp.lang.c Frequently Asked Questions](http://c-faq.com/)

##### Benchmarks #####
* [Benchmarks of the Lockless Memory Allocator][451]
* [Comparison of C/POSIX standard library implementations for Linux][453]
* [Finding the best 64-bit simulation PRNG][454]

##### Beginner Level #####
* [A tutorial on pointers][455]
* [A tutorial on portable Makefiles][456]
* [Building C Projects][457]
* [Introduction to \`fun' C][459]
* [Learning C with GDB][460]
* [POSIX Threads Programming tutorial][462]
* [Templating in C][464]
* [Tutorial on pointers](http://home.netcom.com/~tjensen/ptr/pointers.htm)
* [Building C Projects](http://nethack4.org/blog/building-c.html)
* [C Programming Wikibook](https://en.wikibooks.org/wiki/C_Programming)
* [Introduction to 'fun' C](https://gist.github.com/eatonphil/21b3d6569f24ad164365)
* [Learning C with GDB](https://www.recurse.com/blog/5-learning-c-with-gdb)
* [POSIX Threads Programming tutorial](https://computing.llnl.gov/tutorials/pthreads/) (a little dated, but most of it is still valid and useful)
* [The GNU C Programming Tutorial](http://www.crasseux.com/books/ctut.pdf) (online PDF)
* [Templating in C](http://blog.pkh.me/p/20-templating-in-c.html)
* [Akagi201/learning-cmake](https://github.com/Akagi201/learning-cmake) - learning cmake

##### Intermediate Level #####
* [memcpy vs memmove][461]
* [8 gdb tricks you should know][465]
* [10 C99 tricks][466]
* [A comprehensive MPI tutorial resource][467]
* [Diving into concurrency: trying out mutexes and atomics][468]
* [Generic C reference counting][469]
* [How to write portable C without complicating your build][470]
* [Introduction to OpenMP][471] (video)
* [OpenMP tutorial][472]
* [MPI tutorial][473]
* [Scalable C - Writing Large-Scale Distributed C][474]
* [Some unknown features or tricks in C language][475]
* [What every C programmer should know about undefined behaviour][476]
* [8 gdb tricks you should know](https://blogs.oracle.com/linux/8-gdb-tricks-you-should-know-v2)
* [10 C99 tricks](https://blog.noctua-software.com/c-tricks.html)
* [Diving into concurrency: trying out mutexes and atomics](https://jvns.ca/blog/2014/12/14/fun-with-threads/)
* [Introduction to OpenMP](https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG) (video)
* [OpenMP tutorial](https://computing.llnl.gov/tutorials/openMP/) (for the OpenMP3 standard)
* [memcpy vs memmove](https://web.archive.org/web/20170620131430/https://www.tedunangst.com/flak/post/memcpy-vs-memmove)
* [MPI tutorial](https://computing.llnl.gov/tutorials/mpi/)
* [Some unknown features or tricks in C language](https://proprogramming.org/some-unknown-features-or-tricks-in-c-language/)
* [The lost art of C structure packing](http://www.catb.org/esr/structure-packing/)
* [What a C programmer should know about memory](http://marek.vavrusa.com/memory/)
* [What every C programmer should know about undefined behaviour](http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html)
* [arjun024/hide-data-in-ptr](https://github.com/arjun024/hide-data-in-ptr) - how to hide data inside pointers

##### Advanced Level #####
* [Advanced metaprogramming in C][477]
* [A quick tutorial on implementing and debugging malloc, free, calloc, and realloc][478]
* [Bit twiddling hacks][479]
* [Implementing smart pointers for the C programming language][480]
* [Inline functions in C][481]
* [Metaprogramming custom control structures in C][482]
* [Some dark corners of C][483]
* [Writing efficient C and C code optimization][484]
* [Advanced metaprogramming in C](http://250bpm.com/blog:56)
* [Quick tutorial on implementing and debugging malloc, free, calloc, and realloc](http://danluu.com/malloc-tutorial/)
* [Bit twiddling hacks](https://graphics.stanford.edu/~seander/bithacks.html)
* [I do not know C](https://kukuruku.co/post/i-do-not-know-c/)
* [Implementing smart pointers for the C programming language](https://snai.pe/c/c-smart-pointers/)
* [Inline functions in C](http://www.greenend.org.uk/rjk/tech/inline.html)
* [Metaprogramming custom control structures in C](https://www.chiark.greenend.org.uk/~sgtatham/mp/)
* [Some dark corners of C](https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.gaf50702c_0153)
* [Writing efficient C and C code optimization](https://www.codeproject.com/articles/6154/writing-efficient-c-and-c-code-optimization)
* [What every programmer should know about memory](https://www.akkadia.org/drepper/cpumemory.pdf)

#### Code Examples ####
* [0intro/plan9](https://github.com/0intro/plan9) - Plan 9 from Bell Labs
* [CTurt/Cinoop](https://github.com/CTurt/Cinoop) - Multiplatform Game Boy emulator
* [ChibiOS/ChibiOS](https://github.com/ChibiOS/ChibiOS) - Read only mirror of SVN ChibiOS repository. Official forum http://forum.chibios.org  Bugtracker http://sourceforge.net/projects/chibios
* [EtchedPixels/FUZIX](https://github.com/EtchedPixels/FUZIX) - FuzixOS: Because Small Is Beautiful
* [Fedjmike/mini-c](https://github.com/Fedjmike/mini-c) - Dr Strangehack, or: how to write a self-hosting C compiler in 10 hours
* [FreddieV4/DailyProgrammerChallenges](https://github.com/FreddieV4/DailyProgrammerChallenges) - External Repo of Challenges from r/dailyprogrammer
* [Harvey-OS/harvey](https://github.com/Harvey-OS/harvey) - A distributed operating system
* [HarveyHunt/howm](https://github.com/HarveyHunt/howm) - A lightweight, X11 tiling window manager that behaves like vim
* [HuoLanguage/huo](https://github.com/HuoLanguage/huo) - interpreted language written in C
* [LIJI32/SameBoy](https://github.com/LIJI32/SameBoy) - Game Boy and Game Boy Color emulator written in C
* [LemonBoy/bar](https://github.com/LemonBoy/bar) - A featherweight, lemon-scented, bar based on xcb
* [MagerValp/AsmHeap](https://github.com/MagerValp/AsmHeap) - Heap data structure in 6502 assembler
* [MinhasKamal/CreepyCodeCollection](https://github.com/MinhasKamal/CreepyCodeCollection) - A Nonsense Collection of Disgusting Codes (quine-polyglot-code-golf-obfuscated-signature-creepy-codes-mandelbrot-esoteric-language-esoteric-programming-strange-golfing-spooky-weird)
* [MoarVM/MoarVM](https://github.com/MoarVM/MoarVM) - A VM with adaptive optimization and JIT compilation, built for Rakudo Perl 6
* [RIOT-OS/RIOT](https://github.com/RIOT-OS/RIOT) - RIOT -  The friendly OS for IoT
* [SilverRainZ/OS67](https://github.com/SilverRainZ/OS67) - An unix-like toy kernel.
* [Visgean/Zeus](https://github.com/Visgean/Zeus) - NOT MY CODE! Zeus trojan horse - leaked in 2011, I am not the author. I have created this repository to make the access for study as easy as possible.
* [Wilfred/babyc](https://github.com/Wilfred/babyc) - A toy C compiler
* [adsr/mle](https://github.com/adsr/mle) - flexible terminal-based text editor (C)
* [adtac/fssb](https://github.com/adtac/fssb) - A filesystem sandbox for Linux using syscall intercepts.
* [andreafabrizi/prism](https://github.com/andreafabrizi/prism) - PRISM is an user space stealth reverse shell backdoor, written in pure C.
* [andwn/cave-story-md](https://github.com/andwn/cave-story-md) - A fan port of Cave Story for the Sega Mega Drive
* [angband/angband](https://github.com/angband/angband) - A free, single-player roguelike dungeon exploration game
* [arjun024/mkernel](https://github.com/arjun024/mkernel) - a minimalistic kernel
* [begeekmyfriend/leetcode](https://github.com/begeekmyfriend/leetcode) - LeetCode in pure C
* [bl0ckeduser/new-bpf-tools](https://github.com/bl0ckeduser/new-bpf-tools) - subset-of-C compiler targeting 32-bit x86
* [bovine/datapipe](https://github.com/bovine/datapipe) - Network TCP port forwarding
* [brenns10/lsh](https://github.com/brenns10/lsh) - Simple shell implementation.  Tutorial here ->
* [brho/plan9](https://github.com/brho/plan9) - UC Berkeley release of Plan 9 under the GPLv2
* [caisah/Sedgewick-algorithms-in-c-exercises-and-examples](https://github.com/caisah/Sedgewick-algorithms-in-c-exercises-and-examples) - Examples and exercises from Algorithms in C, Parts 1-4: Fundamentals, Data Structures, Sorting, Searching by Robert Sedgewick book
* [carld/micro-lisp](https://github.com/carld/micro-lisp) - 🎄A very small Lisp programming language 😀that used to be under 200 lines of C🎄
* [ccpalettes/the-c-programming-language-second-edition-solutions](https://github.com/ccpalettes/the-c-programming-language-second-edition-solutions) - Solutions for all exercises in the book "The C Programming Language - Second Edition"(referred to as K&R, after its authors' initials) by Brian W. Kernighan and Dennis M. Ritchie.
* [chelyaev/ffmpeg-tutorial](https://github.com/chelyaev/ffmpeg-tutorial) - A set of tutorials that demonstrates how to write a video player based on FFmpeg
* [chneukirchen/cwm](https://github.com/chneukirchen/cwm) - portable version of OpenBSD's cwm(1) window manager
* [cirosantilli/cpp-cheat](https://github.com/cirosantilli/cpp-cheat) - C, C++, POSIX and Linux system programming minimal examples. Asserts used wherever possible. Hello worlds for cool third party libraries and build systems. Cheatsheets, tutorials and mini-projects.
* [cksystemsteaching/selfie](https://github.com/cksystemsteaching/selfie) - An educational software system of a tiny self-compiling C compiler, a tiny self-executing RISC-V emulator, and a tiny self-hosting RISC-V hypervisor.
* [cmus/cmus](https://github.com/cmus/cmus) - Small, fast and powerful console music player for Unix-like operating systems.
* [collectd/collectd](https://github.com/collectd/collectd) - The system statistics collection daemon. Please send Pull Requests here!
* [conghui/algorithms-in-c](https://github.com/conghui/algorithms-in-c) - Exercise of the book Algorithms In C, Part 1-4, Fundamentals, Data Strcuture, Sorting, Searching, written by  Robert Sedgewick
* [cstack/db_tutorial](https://github.com/cstack/db_tutorial) - Writing a sqlite clone from scratch in C
* [darius/ichbins](https://github.com/darius/ichbins) - A tiny self-hosting Lisp-to-C compiler
* [deadbits/InsecureProgramming](https://github.com/deadbits/InsecureProgramming) - mirror of gera's insecure programming examples | http://community.coresecurity.com/~gera/InsecureProgramming/
* [dimkr/szl](https://github.com/dimkr/szl) - A lightweight, embeddable scripting language
* [dogriffiths/HeadFirstC](https://github.com/dogriffiths/HeadFirstC) - Source code for the book Head First C, by O'Reilly Media
* [drh/cii](https://github.com/drh/cii) - C Interfaces and Implementations
* [eatnumber1/goal](https://github.com/eatnumber1/goal) - g()()()()('al') → "gooooal"
* [espruino/Espruino](https://github.com/espruino/Espruino) - The Espruino JavaScript interpreter - Official Repo
* [fabianishere/brainfuck](https://github.com/fabianishere/brainfuck) - Brainfuck interpreter written in C
* [feeley/gambit](https://github.com/feeley/gambit) - Gambit is an efficient implementation of the Scheme programming language.
* [felixangell/mac](https://github.com/felixangell/mac) - virtual machine in c
* [fragglet/yoctolisp](https://github.com/fragglet/yoctolisp) - Tiny Scheme-like Lisp interpreter written in a weekend
* [freddiev4/DailyProgrammerChallenges](https://github.com/freddiev4/DailyProgrammerChallenges) - External Repo of Challenges from r/dailyprogrammer
* [guilleiguaran/xv6](https://github.com/guilleiguaran/xv6) - mirror of the source code of the Xv6 operating system
* [haldean/x6502](https://github.com/haldean/x6502) - Yet another 6502 emulator that one day dreams of being an Atari 2600.
* [hellerve/e](https://github.com/hellerve/e) - A dead simple editor
* [hoxnox/rawsock_recv_example](https://github.com/hoxnox/rawsock_recv_example) - SOCK_RAW IPPROTO_UDP socket data transmission example
* [i3/i3](https://github.com/i3/i3) - A better tiling and dynamic window manager
* [intellectualheaven/ceed](https://github.com/intellectualheaven/ceed) - A tiny x86 compiler with ELF and PE target
* [irssi/irssi](https://github.com/irssi/irssi) - The client of the future
* [island-org/island](https://github.com/island-org/island) - Lightweight and low-level creative coding toolkits in C.
* [jakogut/tinyflock](https://github.com/jakogut/tinyflock) - A simple, high-performance, threaded, and interactive flocking demo written in C with GLFW.
* [jakogut/tinyvm](https://github.com/jakogut/tinyvm) - TinyVM is a small, fast, lightweight virtual machine written in pure ANSI C.
* [janet-lang/janet](https://github.com/janet-lang/janet) - A dynamic language and bytecode vm
* [jbangert/trapcc](https://github.com/jbangert/trapcc) - Computing with traps
* [jeff-1amstudios/restful-doom](https://github.com/jeff-1amstudios/restful-doom) - HTTP+JSON API hosted inside the 1993 DOOM engine!
* [jelathro/C](https://github.com/jelathro/C) - C Programming Projects
* [jnz/q3vm](https://github.com/jnz/q3vm) - Q3VM - Embeddable bytecode virtual machine/interpreter for C-language input
* [jordansissel/xdotool](https://github.com/jordansissel/xdotool) - fake keyboard/mouse input, window management, and more
* [justinmeza/lci](https://github.com/justinmeza/lci) - A LOLCODE interpreter written in C.
* [kev009/cii](https://github.com/kev009/cii) - libcii ported to Autotools/libtool - D. R. Hanson's C Interfaces and Implementations
* [kevinlawler/kona](https://github.com/kevinlawler/kona) - Open-source implementation of the K programming language
* [kframework/c-semantics](https://github.com/kframework/c-semantics) - Semantics of C in K
* [klange/toaruos](https://github.com/klange/toaruos) - A completely-from-scratch hobby operating system: bootloader, kernel, drivers, C library, and userspace including a composited graphical UI, dynamic linker, syntax-highlighting text editor, network stack, etc.
* [lbrito1/cstuff](https://github.com/lbrito1/cstuff) - Algorithms & data structures in C
* [lennylxx/leetcode](https://github.com/lennylxx/leetcode) - Pure C solution for LeetCode
* [lotabout/write-a-C-interpreter](https://github.com/lotabout/write-a-C-interpreter) - Write a simple interpreter of C. Inspired by c4 and largely based on it.
* [lpsantil/rt0](https://github.com/lpsantil/rt0) - A minimal C runtime for Linux i386 & x86_64
* [marcobambini/gravity](https://github.com/marcobambini/gravity) - Gravity Programming Language
* [mbedmicro/mbed](https://github.com/mbedmicro/mbed) - mbed libraries and tools
* [mgba-emu/mgba](https://github.com/mgba-emu/mgba) - mGBA Game Boy Advance Emulator
* [mil/foo-wm](https://github.com/mil/foo-wm) - A minimal window manager that organizes windows in a tree data structure, provides a socket to send commands to, and nothing more.
* [minix3/minix](https://github.com/minix3/minix) - MINIX 3 (mirror)
* [muennich/sxiv](https://github.com/muennich/sxiv) - Simple X Image Viewer
* [mortdeus/legacy-cc](https://github.com/mortdeus/legacy-cc) - The earliest versions of the very first c compiler known to exist in the wild written by the late legend himself dmr.
* [mruby/mruby](https://github.com/mruby/mruby) - Lightweight Ruby
* [n64dev/cen64](https://github.com/n64dev/cen64) - Cycle-Accurate Nintendo 64 Emulator
* [ndreynolds/flathead](https://github.com/ndreynolds/flathead) - A toy JavaScript interpreter written in C
* [nesbox/tic.computer](https://github.com/nesbox/tic.computer) - 🐛 Public TIC-80 issues tracker
* [nickbjohnson4224/rhombus](https://github.com/nickbjohnson4224/rhombus) - a hobby operating system written in C
* [nickdesaulniers/bf_interpreter_jit_compiler](https://github.com/nickdesaulniers/bf_interpreter_jit_compiler) - Teach myself about interpreters, JITs, and compilers using the Brainfuck language as the toy language
* [paladin-t/my_basic](https://github.com/paladin-t/my_basic) - Lightweight BASIC interpreter written in standard C in dual files. Aimed to be embeddable, extendable and portable.
* [philburk/pforth](https://github.com/philburk/pforth) - Portable Forth in C

#### Courses ####
* [AC-2015-Sem2/DSA-lab](https://github.com/AC-2015-Sem2/DSA-lab) - Data Structures and Algorithms lab repository
* [CoreData/cs50](https://github.com/CoreData/cs50) - CS50 Rep
* [McNopper/OpenGL](https://github.com/McNopper/OpenGL) - OpenGL 3 and 4 with GLSL
* [OpenGLInsights/OpenGLInsightsCode](https://github.com/OpenGLInsights/OpenGLInsightsCode) - Source code for OpenGL Insights
* [RPISEC/MBE](https://github.com/RPISEC/MBE) - Course materials for Modern Binary Exploitation by RPISEC
* [cs3157/recitations](https://github.com/cs3157/recitations) - Recitation notes for cs3157, the C systems programming course with a narrative

--------------------------------------------------------------------------------

## AI ##
Neural nets, machine learning, and other similar things.
* [Cranium][6] - Portable, header-only ANN library in C99. [``MIT``][MIT]
* [FANN][7] - Fast Artifical Neural Network library; an implementation of neural
  networks. [``GPL-2.0-only``][GPL-2.0-only]
* [Genann][8] - Simple ANN in C89, without additional dependencies. [``Zlib``][Zlib]
* [KANN][9] - Two-file ANN library. [``MIT``][MIT]
* [LibDEEP][10] - Deep learning library. [``BSD-3-Clause``][BSD-3-Clause]
* [Darknet](https://pjreddie.com/darknet/) - Open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.
* [100/Cranium](https://github.com/100/Cranium) - 🤖   A portable, header-only, artificial neural network library written in C99
* [2hanson/DecisionTree](https://github.com/2hanson/DecisionTree) - Decision Tree
* [Blei-Lab/lda-c](https://github.com/Blei-Lab/lda-c) - This is a C implementation of variational EM for latent Dirichlet allocation (LDA), a topic model for text or other discrete data.
* [GHamrouni/Recommender](https://github.com/GHamrouni/Recommender) - A C library for product recommendations/suggestions using collaborative filtering (CF)
* [H2CO3/libsprec](https://github.com/H2CO3/libsprec) - C library for speech recognition using the Google Speech API
* [HIPS/Probabilistic-Backpropagation](https://github.com/HIPS/Probabilistic-Backpropagation) - Implementation in C and Theano of the method Probabilistic Backpropagation for scalable Bayesian inference in deep neural networks.
* [JulienPalard/Mine](https://github.com/JulienPalard/Mine) - Little data miner
* [TheWeatherChannel/dClass](https://github.com/TheWeatherChannel/dClass) - Device Classification Engine
* [antirez/shapeme](https://github.com/antirez/shapeme) - Evolve images using simulated annealing
* [attractivechaos/kann](https://github.com/attractivechaos/kann) - A lightweight C library for artificial neural networks
* [cjac/cmusphinx](https://github.com/cjac/cmusphinx) - CMU Sphinx - Speech Recognition Toolkit
* [cmusphinx/pocketsphinx](https://github.com/cmusphinx/pocketsphinx) - PocketSphinx is a lightweight speech recognition engine, specifically tuned for handheld and mobile devices, though it works equally well on the desktop
* [codeplea/genann](https://github.com/codeplea/genann) - simple neural network library in ANSI C
* [dake/openVP](https://github.com/dake/openVP) - Voice Print Recognition in C language.
* [encog/encog-c](https://github.com/encog/encog-c) - The Encog project for C/C++
* [glouw/tinn](https://github.com/glouw/tinn) - The tiny neural network library
* [iunderstand/SWE](https://github.com/iunderstand/SWE) - SWE Toolkit. Learning Semantic Word Embeddings based on Ordinal Knowledge Constraints. A general framework to incorporate semantic knowledge into the popular data-driven learning process of word vectors. Applications including word similarity, sentence completion, etc. ACL-2015 long paper, Beijing, China
* [knossos-project/knossos](https://github.com/knossos-project/knossos) - KNOSSOS is a software tool for the visualization and annotation of 3D image data and was developed for the rapid reconstruction of neural morphology and connectivity.

## Algoritm Implementations ##
* [sort][434] - Collection of sorting routines, which type-specialize at
  compile-time with a user-defined type. [``MIT``][MIT]
* [dlx][418] - Implementation of [Knuth's Algorithm X][419], with example
  solvers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [BigZaphod/AStar](https://github.com/BigZaphod/AStar) - C Implementation of the A* Pathfinding Algorithm
* [uastar][195] - Minimal A\* implementation. [``ZLib``][Zlib]
* [BlackLight/fkmeans](https://github.com/BlackLight/fkmeans) - A tiny library in C for managing kmeans clusterization algorithm over arbitrary data sets, both by manually specifying the number k of clusters and computing it automatically using Schwarz criterion
* [CVLearner/Mixture-of-Gaussians](https://github.com/CVLearner/Mixture-of-Gaussians) - Fit a Gaussian mixture model given a set of data
* [Cyan4973/FiniteStateEntropy](https://github.com/Cyan4973/FiniteStateEntropy) - New generation entropy codecs : Finite State Entropy and Huff0
* [IAIK/CJAG](https://github.com/IAIK/CJAG) - CJAG is an open-source implementation of our cache-based jamming agreement.
* [Kevincav/Radix-Sort](https://github.com/Kevincav/Radix-Sort) - Radix Sort with different data types.
* [Soryusan/Ranking_Algorithm](https://github.com/Soryusan/Ranking_Algorithm) - Ranking algorithm data collector/cruncher
* [TheAlgorithms/C](https://github.com/TheAlgorithms/C) - All Algorithms implemented in C
* [agl/curve25519-donna](https://github.com/agl/curve25519-donna) - Implementations of a fast Elliptic-curve Diffie-Hellman primitive
* [ai-ku/scode](https://github.com/ai-ku/scode) - Sphere embedding (s-code) is a variation of Euclidean embedding of co-occurence data (code).
* [aimxhaisse/des](https://github.com/aimxhaisse/des) - C implementation of Data Encryption Standard
* [ajrisi/fsm](https://github.com/ajrisi/fsm) - A finite state machine engine in C - used as a parser for complex data structures
* [chaoslawful/ccard-lib](https://github.com/chaoslawful/ccard-lib) - C library for estimating cardinality in streams for which it is infeasible to store all events in memory
* [citiususc/BigBWA](https://github.com/citiususc/BigBWA) - Approaching the Burrows-Wheeler Aligner to Big Data Technologies
* [coolwanglu/quantile-alg](https://github.com/coolwanglu/quantile-alg) - Algorithms for finding quantiles of a data stream
* [cvxgrp/scs](https://github.com/cvxgrp/scs) - C package that solves convex cone problems via operator splitting
* [davidreynolds/algorithms](https://github.com/davidreynolds/algorithms) - A repository of assorted algorithms and data structures.
* [dhuertas/AES](https://github.com/dhuertas/AES) - AES algorithm implementation in C
* [duckythescientist/obfuscatedLife](https://github.com/duckythescientist/obfuscatedLife) - Conway's Game of Life in 9 lines of C
* [jmcejuela/Levenshtein-MySQL-UDF](https://github.com/jmcejuela/Levenshtein-MySQL-UDF) - General Levenshtein algorithm and k-bounded levenshtein distance in linear time and constant space. Implementation in C as a MySQL UDF
* [jobovy/extreme-deconvolution](https://github.com/jobovy/extreme-deconvolution) - Density estimation using Gaussian mixtures in the presence of noisy, heterogeneous and incomplete data
* [jrd730/WordFinder](https://github.com/jrd730/WordFinder) - a data structure that specializes in rapidly finding valid anagrams of strings
* [kljensen/Gemoda](https://github.com/kljensen/Gemoda) - A generic motif discovery algorithm for sequential data
* [kokke/tiny-AES-c](https://github.com/kokke/tiny-AES-c) - Small portable AES128/192/256 in C
* [kokke/tiny-AES128-C](https://github.com/kokke/tiny-AES128-C) - Small portable AES128/192/256 in C
* [kroitor/gjk.c](https://github.com/kroitor/gjk.c) - Gilbert-Johnson-Keerthi (GJK) collision detection algorithm in 200 lines of clean plain C
* [kurtisthompson/Algorithms](https://github.com/kurtisthompson/Algorithms) - Random assortment of Interesting data structures and/or algorithms and academic work
* [lacker/ikalman](https://github.com/lacker/ikalman) - An iPhone-friendly Kalman filter written in C.
* [leecarraher/CardinalityShiftClustering](https://github.com/leecarraher/CardinalityShiftClustering) - MOVED -- https://github.com/wilseypa/rphash -- Ongoing research into communication minimizing parallel data clustering for an LSH accelerated random projection mean-shift algorithm.
* [licstar/compare](https://github.com/licstar/compare) - compare embedding
* [mischasan/aho-corasick](https://github.com/mischasan/aho-corasick) - A-C implementation in "C". Tight-packed (interleaved) state-transition matrix -- as fast as it gets, as small as it gets.
* [mmadry/st-hmp](https://github.com/mmadry/st-hmp) - Implementation of the Spatio-Temporal Hierarchical Matching Pursuit (ST-HMP) descriptor presented in the paper: M. Madry, L. Bo, D. Kragic, D. Fox, "ST-HMP: Unsupervised Spatio-Temporal Feature Learning for Tactile Data". In ICRA, 2014 (Download: http://www.nada.kth.se/~madry/publications/madry2014ICRA.pdf).
* [msteinbeck/tinyspline](https://github.com/msteinbeck/tinyspline) - ANSI C library for NURBS, B-Splines, and Bézier curves with interfaces for C++, C#, D, Java, Lua, Octave, PHP, Python, R, and Ruby
* [oap/ekf-angles](https://github.com/oap/ekf-angles) - Extended Kalman Filter for Accelerometer and Gyro data
* [ntamas/plfit](https://github.com/ntamas/plfit) - Fitting power-law distributions to empirical data, according to the method of Clauset, Shalizi and Newman

## Argument Parsing ##
* [parg][410] - A single-file reimplementation of ``getopt`` with better
  defaults. [``CC0-1.0``][CC0-1.0]
* [argparse][411] - Command-line argument parsing library, inspired by Python's
  argparse module. [``MIT``][MIT]
* [docopt.c][412] - Implementation of a command-line option parser. [``MIT``][MIT]
* [PaulStoffregen/teensy_loader_cli](https://github.com/PaulStoffregen/teensy_loader_cli) - Command line Teensy Loader
* [clibs/flag](https://github.com/clibs/flag) - Go-style flag parsing for C
* [clibs/commander](https://github.com/clibs/commander) - Commander option parser ported to C - simple API, auto-generated --help
* [cofyc/argparse](https://github.com/cofyc/argparse) - Command-line arguments parsing library.

## Calculations ##
* [apophenia][250] - Library for statistical and scientific computing. [``GPL-2.0-only``][GPL-2.0-only]
* [Arb][251] - Library for arbitrary-precision interval arithmetic. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [ATLAS][252] - Automatically Tuned Linear Algebra Software. [``BSD-3-Clause``][BSD-3-Clause]
* [clBLAS][253] - BLAS functions written in OpenCL. [``Apache-2.0``][Apache-2.0]
* [cmathl][254] - Math library with a great variety of mathematical functions
  with CMake build support. Seeks to be close to C89/C90 compliant for
  portability. [``MIT``][MIT]
* [Cuba][255] - Library for multidimensional numerical integration. [``LGPL-3.0-only``][LGPL-3.0-only]
* [fft-c][256] - A high-performance Fourier Transform from netlib's fftpack;
  wrapped in a user-friendly format [``MIT``][ MIT]
* [FFTW][257] - The Fastest Fourier Transform in the West; a highly optimized
  fast Fourier transform routine. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [FLINT][258] - Fast Library for Number Theory; a library supporting arithmetic
  with numbers, polynomials, power series and matrices, among others. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [GLPK][259] - GNU Linear Programming Kit; a package designed for solving
  large-scale linear programming, mixed integer programming and other related
  problems. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GMP][260] - GNU Multple Precision Arithmetic Library; a library for
  arbitrary-precision arithmetic. [``GPL-2.0-only``][GPL-2.0-only] or [``LGPL-3.0-only``][LGPL-3.0-only]
* [GNU MPC][261] - Library for complex number arithmetic. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [GNU MPFR][262] - Library for arbitrary-precision floating-point arithmetic. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [GNU MPRIA][263] - Portable mathematics library for multi-precision rational
  interval arithmetic. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GSL][264] - The GNU Scientific Library; a sophisticated numerical library. [``GPL-3.0-only``][GPL-3.0-only].
* [KISS FFT][265] - Simple fast Fourier transform library. [``BSD-3-Clause``][BSD-3-Clause]
* [LAPACKE][266] - Interface to [LAPACK][134]. [``BSD-3-Clause``][BSD-3-Clause]
* [LibTomMath][267] - Portable, number-theoretic, multiple-precision integer
  library. Supports algebra, digit manipulation, modular reductions, and various
  number-theoretic routines. Public domain.
* [LibTomPoly][268] - Polynomial-related maths library. Public domain.
* [PARI/GP][269] - Computer algebra system for number theory; includes a
  compiler to C. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [PETSc][270] - Suite of data structures and routines for scalable parallel
  solution of scientific applications modelled by partial differential
  equations. [``BSD-2-Clause``][BSD-2-Clause]
* [SCS][271] - Splitting Conic Solver; a numerical optimization package for
  solving large-scale convex cone problems. [``MIT``][MIT]
* [SLEPc][272] - Library for the solution of large, sparse eigenvalue
  problems on parallel computers. [``LGPL-3.0-only``][LGPL-3.0-only]
* [TomsFastMath][273] - Set of optimized maths operations (in assembly),
  suitable for cryptographic use. Public domain.
* [Yeppp!][274] - Fast, SIMD-optimized mathematical library. [``BSD-3-Clause``][BSD-3-Clause]
* [tinyexpr][379] - Tiny recursive-descent parser, compiler and evaluation
  engine for simple mathematical expressions. [``BSD-3-Clause``][BSD-3-Clause]
* [apophenia](http://apophenia.info/) - Library for statistical and scientific computing. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [ATLAS](http://math-atlas.sourceforge.net/) - Automatically Tuned Linear Algebra Software. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [BLAS](http://www.netlib.org/blas/) - Basic Linear Algebra Subprograms; a set of routines that provide vector and matrix operations. [`BLAS license`](http://www.netlib.org/blas/#_licensing)
* [CDFLIB](https://people.sc.fsu.edu/~jburkardt/c_src/cdflib/cdflib.html) - Library with routines to evaluate cumulative density functions fo a variety of standard probability distributions.  Also can compute one parameter of the CDF given the others.  (No license given)
* [cmathl](https://scientificc.github.io/cmathl/) - Pure-C Math library with a great variety of mathematical functions and CMake build support. Seeks to be close to C89/C90 compliant for portability. [`MIT`](https://github.com/ScientificC/cmathl/blob/master/LICENSE)
* [Cuba](http://www.feynarts.de/cuba/) - Library for multidimensional numerical integration. [`GNU LGPLv3`](http://www.gnu.org/licenses/lgpl.html)
* [FFTW](http://www.fftw.org/) - The Fastest Fourier Transform in the West; a highly-optimized fast Fourier transform routine. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [FLINT](http://flintlib.org/) - Fast Library for Number Theory; a library supporting arithmetic with numbers, polynomials, power series and matrices, among others. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [GLPK](https://www.gnu.org/software/glpk/) - GNU Linear Programming Kit; a package designed for solving large-scale linear programming, mixed integer programming and other related problems. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GMP](https://gmplib.org/) - GNU Multple Precision Arithmetic Library; a library for arbitrary-precision arithmetic. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html) and [`GNU LGPLv3`](http://www.gnu.org/licenses/lgpl.html)
* [GNU MPC](http://www.multiprecision.org/mpc/) - Library for complex number arithmetic. [`GNU LGPL3 or later`](http://www.gnu.org/licenses/lgpl.html)
* [GNU MPFR](https://www.mpfr.org/index.html) - Library for arbitrary-precision floating-point arithmetic. [`GNU LGPL3 or later`](http://www.gnu.org/licenses/lgpl.html) or [`GNU LGPL2.1 or later (until version 2.4.x)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [GNU MPRIA](https://www.gnu.org/software/mpria/) - Portable mathematics library for multi-precision rational interval arithmetic. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GSL](http://www.gnu.org/software/gsl/) - The GNU Scientific Library; a sophisticated numerical library. [`GNU GPL3`](http://www.gnu.org/licenses/gpl.html)
* [igraph](https://igraph.org/) - Library for creating and manipulating large graphs. [`GNU GPL2`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [KISS FFT](https://sourceforge.net/projects/kissfft/) - Very simple fast Fourier transform library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [LAPACKE](http://www.netlib.org/lapack/lapacke.html) - C interface to [LAPACK](http://www.netlib.org/lapack/). [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [PARI/GP](http://pari.math.u-bordeaux.fr/) - Computer algebra system for number theory; includes a compiler to C. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [PETSc](https://www.mcs.anl.gov/petsc/) - Suite of data structures and routines for scalable parallel solution of scientific applications modelled by partial differential equations. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [PROB](https://people.sc.fsu.edu/~jburkardt/c_src/prob/prob.html) - Library that handles various discrete and continuous probability density functions.  [`GNU LGPL3`](https://people.sc.fsu.edu/~jburkardt/txt/gnu_lgpl.txt)
* [Yeppp!](https://bitbucket.org/MDukhan/yeppp) - Very fast, SIMD-optimized mathematical library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [gjrand](https://sourceforge.net/projects/gjrand/) - Library of random-number generation routines. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html) or [`GNU GPLv3`](http://www.gnu.org/licenses/gpl.html)
* [FFTW/fftw3](https://github.com/FFTW/fftw3) - This is the official repository for the FFTW Fourier transform library, version 3.x
* [HdrHistogram/HdrHistogram_c](https://github.com/HdrHistogram/HdrHistogram_c) - C port of the HdrHistogram
* [JuliaMath/openlibm](https://github.com/JuliaMath/openlibm) - High quality system independent, portable, open source libm implementation
* [KhronosGroup/OpenCL-Headers](https://github.com/KhronosGroup/OpenCL-Headers) - Khronos OpenCL-Headers
* [Lichtso/CCWT](https://github.com/Lichtso/CCWT) - Complex Continuous Wavelet Transformation
* [NCrashed/bzip2](https://github.com/NCrashed/bzip2) - Bindings for bzip2 library, a freely available, patent free, high-quality data compressor.
* [PetteriAimonen/libfixmatrix](https://github.com/PetteriAimonen/libfixmatrix) - C library for fixed point matrix, quaternion and vector calculations
* [b-k/apophenia](https://github.com/b-k/apophenia) - A C library for statistical and scientific computing
* [canonizer/libgpuvm](https://github.com/canonizer/libgpuvm) - library which simplifies host-GPU data transfer using userspace pagefault handling
* [clMathLibraries/clBLAS](https://github.com/clMathLibraries/clBLAS) - a software library containing BLAS functions written in OpenCL
* [clMathLibraries/clRNG](https://github.com/clMathLibraries/clRNG) - an OpenCL based software library containing random number generation functions
* [emrainey/OpenCL-Environment](https://github.com/emrainey/OpenCL-Environment) - A series of utilities aimed at making OpenCL easier to use. Includes clCompiler which generates both binary outputs and precompiled headers which can be used in conjunction with clEnvironment. clQuery allows you to print all known information about a OpenCL data type. clPid, clYUV clImgFilter are all examples of how to use the utilities to create a compile time kernel make it a dependency in you makefiles and then use the clEnvironment to call your kernel.
* [fredrik-johansson/arb](https://github.com/fredrik-johansson/arb) - C library for arbitrary-precision interval arithmetic
* [freshcode/MFMathLib](https://github.com/freshcode/MFMathLib) - A mathematical library providing basic math operations on data types from 8-bits to 1024-bits with overflow/underflow tracking.
* [google/clspv](https://github.com/google/clspv) - Clspv is a prototype compiler for a subset of OpenCL C to Vulkan compute shaders
* [imneme/pcg-c-basic](https://github.com/imneme/pcg-c-basic) - PCG — Minimal C Implementation
* [imneme/pcg-c](https://github.com/imneme/pcg-c) - PCG — C Implementation
* [karrenberg/wfvopencl](https://github.com/karrenberg/wfvopencl) - IMPORTANT NOTICE: This implementation is long outdated. The latest wfvopencl will be made publicly available with the new libwfv implementation. WFVOpenCL is an OpenCL driver for CPUs on the basis of LLVM. This driver employs Whole-Function Vectorization (WFV) in addition to multi-threading to fully exploit the available data-parallelism by executing as many kernel instances in parallel as possible.
* [libtom/libtommath](https://github.com/libtom/libtommath) - LibTomMath is a free open source portable number theoretic multiple-precision integer library written entirely in C.
* [libtom/tomsfastmath](https://github.com/libtom/tomsfastmath) - TomsFastMath is a fast public domain, open source, large integer arithmetic library written in portable ISO C.

## Compression ##
* [blosc][25] - Fast, multi-threaded, meta-compressor library. Various licenses,
  all open source.
* [Brotli][26] - General-purpose lossless compression algorithm library. Has
  speeds comparable to DEFLATE, but much higher compression ratios. [``MIT``][MIT].
* [clzip][27] - C [lzip][28] implementation. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [CRoaring][29] - C implementation of [Roaring bitmaps][30]. [``Apache-2.0``][Apache-2.0]
* [FiniteStateEntropy][31] - Two efficient compression codecs optimized for
  modern CPUs. [``BSD-2-Clause``][BSD-2-Clause]
* [DENSITY][32] - Fast compression library. [``BSD-3-Clause``][BSD-3-Clause]
* [heatshrink][33] - Data compression/decompression library for embedded and
  real-time systems. [``ISC``][ISC]
* [fast\_zlib][34] - Improved zlib, which runs 2 to 10 times faster. [``BSD-3-Clause``][BSD-3-Clause]
* [huffandpuff][35] - Minimal Huffman encoder and decoder. Public domain.
* [libbzip2][36] - Patent-free, high-quality data compression library. [``BSD-4-Clause``][BSD-4-Clause]
* [Lizard][37] - Formerly LZ5. Achieves compression ratios comparable with zip
  and zlib at decompression speeds of 1000MB/s and faster. [``BSD-2-Clause``][BSD-2-Clause]
* [lz4][38] - Fast compression algorithm. [``BSD-2-Clause``][BSD-2-Clause]
* [lzo][39] - Fast data compression library. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [pixz][40] - Parallel, indexed xz compressor. [``BSD-2-Clause``][BSD-2-Clause]
* [shoco][41] - Compressor for small text strings. [``MIT``][MIT]
* [SIMDComp][42] - Simple library for compressing lists of integers using
  binary packing. Makes use of SIMD instructions on x86. [``BSD-3-Clause``][BSD-3-Clause]
* [smaz][43] - Efficient string compression library. [``BSD-3-Clause``][BSD-3-Clause]
* [squash][44] - Compression abstraction library, complete with some utilities. [``MIT``][MIT]
* [TurboPFor][45] - Fast integer compression. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [TurboRLE][46] - Efficient run-length encoding. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [zip][47] - Small zip archive processing library. [``Unlicense``][Unlicense]
* [Zlib][48] - Popular compression library. [``BSD-3-Clause``][BSD-3-Clause]
* [libarchive][49] - libarchive is a portable, efficient C library that can read
  and write streaming archives in a variety of formats. [``BSD-3-Clause``][BSD-3-Clause]
* [zlib-ng][50] - Zlib replacement with optimizations for modern CPUs systems. [``BSD-3-Clause``][BSD-3-Clause]
* [Zstandard][51] - Fast, lossless compression algorithm, targeting real-time
  compression scenarios at zlib-level or better compression ratios. [``BSD-3-Clause``][BSD-3-Clause]
* [libzip](https://libzip.org/) - A C library for reading, creating, and modifying zip archives. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [lzo](http://www.oberhumer.com/opensource/lzo/) - Very fast data compression library. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [zlib](http://zlib.net/) - Massively-spiffy yet delicately-unobtrusive compression library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [bzip2](http://www.bzip.org/) - Patent free, high quality data compressor. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [lz4](https://lz4.github.io/lz4/) - Fast Compression algorithm.
* [snappy](https://github.com/google/snappy) - Fast compression library (implementation in C++, native bindings to C).
* [zstd](http://facebook.github.io/zstd/) - Fast real-time compression algorithm [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [brotli](https://github.com/google/brotli) - Generic lossless compression algorithm based on LZ77, Huffman coding and 2nd order context modelling [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [quicklz](http://www.quicklz.com/index.php) - Fast compression library. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [pixz](https://github.com/vasi/pixz) - Pixz (pronounced pixie) is a parallel, indexing version of `xz`. [`2-clause BSD`](https://directory.fsf.org/wiki/License:BSD-2-Clause)
* [Blosc/c-blosc](https://github.com/Blosc/c-blosc) - A blocking, shuffling and loss-less compression library that can be faster than `memcpy()`.
* [Cyan4973/lz4](https://github.com/Cyan4973/lz4) - Extremely Fast Compression algorithm
* [Cyan4973/zstd](https://github.com/Cyan4973/zstd) - Zstandard - Fast and efficient compression algorithm
* [Dead2/zlib-ng](https://github.com/Dead2/zlib-ng) - zlib replacement with optimizations for "next generation" systems.
* [IlyaGrebnov/libbsc](https://github.com/IlyaGrebnov/libbsc) - High performance block-sorting data compression library
* [RoaringBitmap/CRoaring](https://github.com/RoaringBitmap/CRoaring) - Roaring bitmaps in C (and C++)
* [adnanozsoy/CUDA_Compression](https://github.com/adnanozsoy/CUDA_Compression) - A GPU-based LZSS compression algorithm, highly tuned for NVIDIA GPGPUs and for streaming data, leveraging the respective strengths of CPUs and GPUs together.
* [andikleen/snappy-c](https://github.com/andikleen/snappy-c) - C port of the snappy compressor
* [antirez/smaz](https://github.com/antirez/smaz) - Small strings compression library
* [atomicobject/heatshrink](https://github.com/atomicobject/heatshrink) - data compression library for embedded/real-time systems
* [centaurean/density](https://github.com/centaurean/density) - Superfast compression library
* [kiyo-masui/bitshuffle](https://github.com/kiyo-masui/bitshuffle) - Filter for improving compression of typed binary data.
* [kuba--/zip](https://github.com/kuba--/zip) - A portable, simple zip library written in C
* [lemire/simdcomp](https://github.com/lemire/simdcomp) - A simple C library for compressing lists of integers using binary packing
* [libarchive/libarchive](https://github.com/libarchive/libarchive) - Multi-format archive and compression library
* [lz4/lz4](https://github.com/lz4/lz4) - Extremely Fast Compression algorithm
* [madler/zlib](https://github.com/madler/zlib) - A massively spiffy yet delicately unobtrusive compression library.
* [mist64/pucrunch](https://github.com/mist64/pucrunch) - pucrunch, an Optimizing Hybrid LZ77 RLE Data Compression Program for C64/C128/VIC-20/Plus4
* [moinakg/pcompress](https://github.com/moinakg/pcompress) - A Parallelized Data Deduplication and Compression utility

## Concurrency and Parallelism ##
* [cchan][52] - Small library for channel constructs for inter-thread
  communication. Public domain.
* [checkedthreads][53] - A simple library for parallelism, with built-in
  checking for race conditions. [``BSD-2-Clause``][BSD-2-Clause]
* [ck][54] - Concurrency primitives, safe memory reclamation mechanisms and
  non-blocking data structures. [``BSD-2-Clause``][BSD-2-Clause]
* [FCFS RWLock][55] - First-come first-served Readers/Writers lock for POSIX
  threads. Various licenses, all open source.
* [libconcurrent][56] - Concurrent programming library, using coroutines, for
  C11. [``Zlib``][Zlib]
* [libdill][57] - Library which makes structured concurrent programming easy. [``MIT``][MIT]
* [liburcu][59] - Data synchronization library, which scales linearly with the
  number of cores. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [mill][60] - Go-style concurrency. [``MIT``][MIT]
* [oclkit][61] - Two-file OpenCL wrapper. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [OCL-MLA][62] - OpenCL Mid-Level Abstractions. [``BSD-3-Clause``][BSD-3-Clause]
* [OpenMP][63] - Set of pragmas designed to allow for easy parallelization of
  code. Standard (licensing not applicable).
* [OpenMPI][64] - Message passing interface implementation. [``BSD-3-Clause``][BSD-3-Clause]
* [pth][66] - Portable implementation for non-preemptive priority-based
  scheduling for multiple threads of execution. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [pthreads][67] - POSIX thread library. Standard (no license applicable).
* [TinyCThread][68] - Portable, small implementation of the C11 threads API. [``Zlib``][Zlib]
* [cchan](http://repo.hu/projects/cchan/) - Small library for channel constructs for inter-thread communication. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [ck](http://concurrencykit.org/) - Concurrency primitives, safe memory reclamation mechanisms and non-blocking data structures. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [mill](http://libmill.org/) - Go-style concurrency in C. [`X11`](https://directory.fsf.org/wiki/License:X11)
* [libdill](http://libdill.org/) - Structured concurrency in C. [`X11`](https://directory.fsf.org/wiki/License:X11)
* [MPICH](http://www.mpich.org/) - Another implementation of MPI. [`MPICH licence`](http://git.mpich.org/mpich.git/blob_plain/6aab201f58d71fc97f2c044d250389ba86ac1e3c:/COPYRIGHT)
* [OpenMP](https://www.openmp.org/) - Set of C pragmas designed to allow for easy parallelization of code. [`3-clause BSD`](https://opensource.org/licenses/BSD-3-Clause)
* [OpenMPI](https://github.com/open-mpi/ompi) - Message passing interface implementation. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [pth](https://www.gnu.org/software/pth/) - Portable implementation for non-preemptive priority-based scheduling for multiple threads of execution. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [pthreads](https://en.wikipedia.org/wiki/POSIX_Threads) - The POSIX thread library.
* [SLEPc](https://bitbucket.org/slepc/slepc) - Software library for the solution of large, sparse eigenvalue problems on parallel computers. [`GNU LGPL3`](http://www.gnu.org/licenses/lgpl.html)
* [TinyCThread](https://tinycthread.github.io/) - Portable, small implementation of the C11 threads API. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [cf4ocl](https://fakenmc.github.io/cf4ocl/) - The C Framework for OpenCL; a cross-platform object-oriented framework for developing and benchmarking  [OpenCL](https://www.khronos.org/opencl/) projects. [`GNU LGPL3 (library)`](http://www.gnu.org/licenses/lgpl.html) or [`GNU GPL3 (project code)`](http://www.gnu.org/licenses/gpl.html)
* [Pithikos/C-Thread-Pool](https://github.com/Pithikos/C-Thread-Pool) - A minimal but powerful thread pool in ANSI C
* [baruch/libwire](https://github.com/baruch/libwire) - User space threading (aka coroutines) library for C resembling GoLang and goroutines
* [bjoernknafla/amp](https://github.com/bjoernknafla/amp) - C portable low-level assemblies for parallelism and threading
* [bjoernknafla/peak](https://github.com/bjoernknafla/peak) - Parallelism exploration assembly kit. C toolkit to experiment with task- and data-parallelism.
* [cloudwu/coroutine](https://github.com/cloudwu/coroutine) - A asymmetric coroutine library for C.
* [concurrencykit/ck](https://github.com/concurrencykit/ck) - Concurrency primitives, safe memory reclamation mechanisms and non-blocking (including lock-free) data structures designed to aid in the research, design and implementation of high performance concurrent systems developed in C99+.
* [cudpp/cudpp](https://github.com/cudpp/cudpp) - CUDA Data Parallel Primitives Library
* [etmc/lemon](https://github.com/etmc/lemon) - Lemon is an MPI parallel I/O library that is intended to allow for efficient parallel I/O of both binary and metadata on massively parallel architectures. Data is stored in the SciDAC Lattice QCD Interchange Message Encapsulation format, that allows for storing large blocks of binary data and corresponding metadata in the same file.
* [geertj/cgreenlet](https://github.com/geertj/cgreenlet) - Coroutines for C/C++
* [halayli/lthread](https://github.com/halayli/lthread) - lthread, a multicore enabled coroutine library written in C
* [hnes/libaco](https://github.com/hnes/libaco) - A blazing fast and lightweight C asymmetric coroutine library  💎 ⛅🚀⛅🌞
* [jtsiomb/c11threads](https://github.com/jtsiomb/c11threads) - Trivial C11 threads.h implementation over POSIX threads.
* [kev009/Concurrency-Kit](https://github.com/kev009/Concurrency-Kit) - Concurrency primitives and lock-less data structures
* [matianfu/FUNK](https://github.com/matianfu/FUNK) - a c continuation library inspired by Adam Dunkel's ProtoThread.
* [mbrossard/threadpool](https://github.com/mbrossard/threadpool) - A simple C Thread pool implementation
* [mit-carbon/Flat-Combining](https://github.com/mit-carbon/Flat-Combining) - Traditional data-structure designs, whether lock-based or lock-free, provide parallelism via fine grained synchronization among threads. Flat Combining is a new, efficient synchronization paradigm based on coarse locking.
* [oneoo/alilua-coevent-module](https://github.com/oneoo/alilua-coevent-module) - epoll base coroutine module

## Crypto ##
Mostly library implementations of well-known cryptographic algorithms or
protocols.
* [GNU SASL][69] - Implementation of the Simple Authentication and Security
  Layer and few common SASL mechanisms. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GnuTLS][70] - Secure communication library, implementing SSL, TLS and DTLS. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libgcrypt][71] - General-purpose cryptography library, with a range of
  available ciphers. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [OpenSSL][72] - Implementation of the SSL and TLS protocols. Also includes a
  cryptography library. [Dual Licensed under the OpenSSL License and the SSLeay License][73].
* [liboqs][74] - Library for quantum-resistant cryptographicl algorithms. [``MIT``][MIT]
* [libsodium][75] - Modern and easy-to-use crypto library. [``MIT``][MIT]
* [libtomcrypt][76] - Fairly comprehensive, modular and portable cryptographic
  toolkit. Public domain.
* [mbed TLS][77] - Another crypto implementation. [``Apache-2.0``][Apache-2.0]
* [MIRACL][78] - Multiprecision Integer and Rational Arithmetic Cryptographic
  Library; an SDK for elliptic curve cryptography. [``AGPL-3.0-or-later``][AGPL-3.0-or-later]
* [retter][79] - Collection of hash functions, ciphers, tools, libraries and
  materials related to cryptography and security. Public domain.
* [s2n][80] - C99 implementation of the TLS/SSL protocols, designed to be
  simple, fast and with security as a priority. [``Apache-2.0``][Apache-2.0]
* [sphlib][81] - Set of implementations of various hash functions, including
  several cryptographic ones. [``MIT``][MIT]
* [trezor-crypto][82] - Heavily optimized crypto algorithms for embedded
  devices. [``MIT``][MIT]
* [GnuTLS](https://www.gnutls.org/) - Secure communication library, implementing SSL, TLS and DTLS. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libgcrypt](https://gnupg.org/related_software/libgcrypt/) - General-purpose cryptography library, with a range of available ciphers. [`GNU LGPL2.1or later (code)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) and [`GNU GPL2.1 or later (manual and tools)`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [OpenSSL](https://www.openssl.org/) - Implementation of the SSL and TLS protocols, and also includes a cryptography library. [`Dual Licensed under the OpenSSL License and the SSLeay License`](https://www.openssl.org/source/license.html)
* [libsodium](https://download.libsodium.org/doc/) - Modern and easy-to-use crypto library. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libtomcrypt](https://www.libtom.net/) - Fairly comprehensive, modular and portable cryptographic toolkit. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [mbed TLS](https://tls.mbed.org/) - Another crypto implementation for C. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [libressl](https://www.libressl.org/) - Modernized fork of OpenSSL. [`Various Licenses`](https://cvsweb.openbsd.org/cgi-bin/cvsweb/~checkout~/src/lib/libssl/LICENSE?rev=1.12)
* [jedisct1/libsodium](https://github.com/jedisct1/libsodium) - A modern, portable, easy to use crypto library
* [ARMmbed/mbedtls](https://github.com/ARMmbed/mbedtls) - An open source, portable, easy to use, readable and flexible SSL library
* [B-Con/crypto-algorithms](https://github.com/B-Con/crypto-algorithms) - Basic implementations of standard cryptography algorithms, like AES and SHA-1.
* [CertiVox/MIRACL](https://github.com/CertiVox/MIRACL) - MIRACL Cryptographic SDK: Multiprecision Integer and Rational Arithmetic Cryptographic Library is a C software library that is widely regarded by developers as the gold standard open source SDK for elliptic curve cryptography (ECC).
* [WickrInc/wickr-crypto-c](https://github.com/WickrInc/wickr-crypto-c) - An implementation of the Wickr Secure Messaging Protocol in C
* [ashwinraghav/Parallel_Open_SSL](https://github.com/ashwinraghav/Parallel_Open_SSL) - Use your idle GPU to encrypt your data. Give your CPU some breathing time!
* [awslabs/s2n](https://github.com/awslabs/s2n) - s2n : an implementation of the TLS/SSL protocols
* [bitcoin-core/secp256k1](https://github.com/bitcoin-core/secp256k1) - Optimized C library for EC operations on curve secp256k1
* [bitcoin/secp256k1](https://github.com/bitcoin/secp256k1) - Optimized C library for EC operations on curve secp256k1
* [cloudflare/keyless](https://github.com/cloudflare/keyless) - CloudFlare's Keyless SSL Server Reference Implementation
* [ctz/cifra](https://github.com/ctz/cifra) - A collection of cryptographic primitives targeted at embedded use.
* [cyassl/cyassl](https://github.com/cyassl/cyassl) - Please use wolfSSL now instead: https://github.com/wolfSSL/wolfssl . CyaSSL is a small, fast, portable implementation of TLS/SSL for embedded devices to the cloud.
* [eduardsui/tlse](https://github.com/eduardsui/tlse) - Single C file TLS 1.2/1.3 implementation, using tomcrypt as crypto library
* [h2o/picotls](https://github.com/h2o/picotls) - TLS 1.3 implementation in C (master supports RFC8446 as well as draft-26, -27, -28)
* [jedisct1/libhydrogen](https://github.com/jedisct1/libhydrogen) - A lightweight, secure, easy-to-use crypto library suitable for constrained environments.
* [libressl-portable/portable](https://github.com/libressl-portable/portable) - LibreSSL Portable itself. This includes the build scaffold and compatibility layer that builds portable LibreSSL from the OpenBSD source code.
* [libtom/libtomcrypt](https://github.com/libtom/libtomcrypt) - LibTomCrypt is a fairly comprehensive, modular and portable cryptographic toolkit that provides developers with a vast array of well known published block ciphers, one-way hash functions, chaining modes, pseudo-random number generators, public key cryptography and a plethora of other routines.
* [maciejczyzewski/retter](https://github.com/maciejczyzewski/retter) - A collection of hash functions, ciphers, tools, libraries, and materials related to cryptography. :closed_lock_with_key:
* [mikeryan/crackle](https://github.com/mikeryan/crackle) - Crack and decrypt BLE encryption
* [miracl/MIRACL](https://github.com/miracl/MIRACL) - MIRACL Cryptographic SDK: Multiprecision Integer and Rational Arithmetic Cryptographic Library is a C software library that is widely regarded by developers as the gold standard open source SDK for elliptic curve cryptography (ECC).
* [open-quantum-safe/liboqs](https://github.com/open-quantum-safe/liboqs) - C library for quantum-resistant cryptographic algorithms.

## Databases ##
* [BerkeleyDB][83] - Library for a high-performance embedded database for
  key-value data. [``AGPL-3.0-only``][AGPL-3.0-only]
* [Groonga][84] - Columnar store with full-text search. [``LGPL-2.1-only``][LGPL-2.1-only]
* [Hiredis][85] - Minimalistic client library for Redis. [``BSD-3-Clause``][BSD-3-Clause]
* [libmongoc][86] - High-performance client library for MongoDB. [``Apache-2.0``][Apache-2.0]
* [LMDB][87] - Ultra-fast, ultra-compact key-value embedded data store. [``OLDAP-2.8``][OLDAP-2.8]
* [PostgreSQL][88] - Powerful object-relational database system. [``PostgreSQL``][PostgreSQL]
* [Redis][89] - Advanced key-value store. [``BSD-3-Clause``][BSD-3-Clause]
* [sophia][90] - Modern, embeddable key-value database. [``BSD-2-Clause``][BSD-2-Clause]
* [sparkey][91] - Simple constant key/value storage library. Designed for
  read-heavy loads with infrequent, large bulk inserts. [``Apache-2.0``][Apache-2.0]
* [SQLite][92] - Self-contained, serverless, zero-configuration, transactional
  SQL database engine. Public domain.
* [UnQLite][93] - Self-contained, serverless, zero-configuration, transactional
  NoSQL engine. [``BSD-2-Clause``][BSD-2-Clause]
* [WhiteDB][94] - Lightweight database library, operating entirely in main
  memory. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [BerkeleyDB](https://www.oracle.com/database/berkeley-db/) - Library for a high-performance embedded database for key-value data. [`GNU AGPLv3`](https://www.gnu.org/licenses/agpl.html)
* [Hiredis](https://github.com/redis/hiredis) - Minimalistic client library for Redis. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [LMDB](https://github.com/LMDB/lmdb) - Ultra-fast, ultra-compact key-value embedded data store. [`OpenLDAP License`](https://directory.fsf.org/wiki/License:OLDAP-2.7)
* [MariaDB](https://mariadb.com/) - Robust, scalable and reliable SQL server, designed to be a drop-in replacement for MySQL. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [mongo-c-driver](http://mongoc.org/) - High-performance client library for [MongoDB](https://www.mongodb.com/). [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [PostgreSQL](https://www.postgresql.org/) - Powerful object-relational database system. [`PostgreSQL licence`](https://opensource.org/licenses/postgresql)
* [recutils](https://www.gnu.org/software/recutils/) - Set of tools and a C library for accessing human-editable, plaintext database files called recfiles. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [Redis](https://redis.io/) - Advanced key-value store. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [sophia](http://sophia.systems/) - Modern, embeddable key-value database. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [SQLite](https://www.sqlite.org/about.html) - Self-contained, serverless, zero-configuration, transactional SQL database engine with a C interface. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [UnQLite](https://unqlite.org/) - Self-contained, serverless, zero-configuration, transactional NoSQL engine with a C interface. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [Akash91/CoSQL](https://github.com/Akash91/CoSQL) - A Co-Relational Key-Value Data Store
* [Amaury/FineDB](https://github.com/Amaury/FineDB) - High-performance nosql database. Written in C, multi-threaded, based on LightningDB and nanomsg.
* [BohuTANG/nessDB](https://github.com/BohuTANG/nessDB) - A very fast transactional key-value, embedded database storage engine.
* [GNOME/libgda](https://github.com/GNOME/libgda) - Libgda is a (relatively small) database access library:
* [Qihoo360/Atlas](https://github.com/Qihoo360/Atlas) - A high-performance and stable proxy for MySQL
* [Softmotions/ejdb](https://github.com/Softmotions/ejdb) - EJDB — Embeddable JSON Database engine
* [Suor/postgresql-json](https://github.com/Suor/postgresql-json) - Extract data from PostgreSQL JSON fields.
* [aerospike/aerospike-client-c](https://github.com/aerospike/aerospike-client-c) - Aerospike C Client
* [aerospike/aerospike-server](https://github.com/aerospike/aerospike-server) - Aerospike Database Server – flash-optimized, in-memory, nosql database
* [antirez/redis](https://github.com/antirez/redis) - Redis is an in-memory database that persists on disk. The data model is key-value, but many different kind of values are supported: Strings, Lists, Sets, Sorted Sets, Hashes, HyperLogLogs, Bitmaps.
* [bcmpinc/dagdb](https://github.com/bcmpinc/dagdb) - small database for storing semi-structured data
* [cloudwu/lua-db](https://github.com/cloudwu/lua-db) - A database shared data among multi-states .
* [edussx/database](https://github.com/edussx/database) - B+tree database
* [fictorial/logstore](https://github.com/fictorial/logstore) - experimental data storage engine for arbitrary data for POSIX systems with spinning hard disks
* [grahamking/Key-Value-Polyglot](https://github.com/grahamking/Key-Value-Polyglot) - A basic key-value store, repeated in C, Go, Python (basic, gevent, and diesel), Ruby (event machine), Java, Scala, Haskell, and NodeJS.
* [kbranigan/pow](https://github.com/kbranigan/pow) - C datastore/cache for MySQL data
* [lfittl/libpg_query](https://github.com/lfittl/libpg_query) - C library for accessing the PostgreSQL parser outside of the server environment
* [maciejczyzewski/hashbase](https://github.com/maciejczyzewski/hashbase) - A fast, efficient on-disk/in-memory database with many different kind of data structures. :floppy_disk:
* [maxmind/libmaxminddb](https://github.com/maxmind/libmaxminddb) - C library for the MaxMind DB file format
* [mfragkoulis/PiCO_QL](https://github.com/mfragkoulis/PiCO_QL) - SQL query interface to C++ collections and C data structures. Also configurable as a loadable Linux kernel module and an extension to Valgrind tools.
* [mongodb/mongo-c-driver-legacy](https://github.com/mongodb/mongo-c-driver-legacy) - C Driver for MongoDB
* [mongodb/mongo-c-driver](https://github.com/mongodb/mongo-c-driver) - A high-performance MongoDB driver for C

## Data Structures and Types ##
* [libhl][58] - Library implementing a thread-safe API to manage a range of data
  structures. Also provides some supporting functions and structures for
  concurrent and lockfree programming. [``LGPL-3.0-only``][LGPL-3.0-only]
* [Collections-C][95] - Library of generic data structures. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [kdtree][96] - Simple library for working with KD-trees. [``BSD-3-Clause``][BSD-3-Clause]
* [libavl][97] - Library containing a range of self-balancing binary trees. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [ds][98] - Common Data Structures and Algorithms. [``MIT``][MIT]
* [igraph][99] - A graph processing library. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [liblfds][100] - Portable lock-free data structure library. Public domain
  (more exactly, whatever license you want).
* [M\*LIB][101] - Library for generic, but typesafe C containers. Implemented as
  header-only. [``BSD-2-Clause``][BSD-2-Clause]
* [offbrand][102] - Collection of generic, reference-counted data structures. [``MIT``][MIT]
* [libsrt][103] - Soft and hard real-time data structures. [``BSD-3-Clause``][BSD-3-Clause].
* [list.h][104] - Implementations for single- and double-linked list functions. [``GPL-3.0-only``][GPL-3.0-only]
* [PackedArray][105] - Random-access array of tightly packed unsigned integers
of any desired width. Has a SIMD-optimized implementation. [``WTFPL``][WTFPL]
* [uthash][106] - Single-file hash table implementation. [``BSD-1-Clause``][BSD-1-Clause]
* [vector.h][107] - Header library for typed lists. [``MIT``][MIT]
* [20centaurifux/datatypes](https://github.com/20centaurifux/datatypes) - A collection of various datatypes in C (linked lists, stack, queue, red-black tree and hash table).
* [2ion/libqueue](https://github.com/2ion/libqueue) - C library providing persistent, named data storage queues
* [Achoulos/Data-Structures](https://github.com/Achoulos/Data-Structures) - Implementation of Data Structures and Sorts in C
* [Blosc/bcolz](https://github.com/Blosc/bcolz) - A columnar data container that can be compressed.
* [ClickerMonkey/CDSL](https://github.com/ClickerMonkey/CDSL) - A data structure library written in C
* [DanielWaterworth/Butterfly](https://github.com/DanielWaterworth/Butterfly) - [DEPRECATED] Butterfly is a C library that implements a very simple 'dynamic' data-type. It could be used, for example, to manipulate JSON data from C. It is distributed under LGPL.
* [Incarnation-p-lee/libds](https://github.com/Incarnation-p-lee/libds) - unified data structure implementation lib of C
* [Krakonos/cutils](https://github.com/Krakonos/cutils) - C utilities and data structures
* [LPD-EPFL/ASCYLIB](https://github.com/LPD-EPFL/ASCYLIB) - ASCYLIB is a concurrent-search data-structure library with over 30 implementantions of linked lists, hash tables, skip lists, and binary search trees.
* [MichaelJWelsh/cdsa](https://github.com/MichaelJWelsh/cdsa) - A library of generic intrusive data structures and algorithms in ANSI C
* [Tarsnap/kivaloo](https://github.com/Tarsnap/kivaloo) - Kivaloo is a collection of utilities which together form a data store associating keys of up to 255 bytes with values of up to 255 bytes.
* [ZSShen/C-Common-Data-Structures](https://github.com/ZSShen/C-Common-Data-Structures) - Uniform C APIs for data structure manipulation
* [agl/critbit](https://github.com/agl/critbit) - Critbit trees in C
* [alexanderb14/cCollections](https://github.com/alexanderb14/cCollections) - lightweight dynamic data structures for C
* [angelortega/mpdm](https://github.com/angelortega/mpdm) - Minimum Profit Data Manager
* [antirez/rax](https://github.com/antirez/rax) - A radix tree implementation in ANSI C
* [argv0/nbds](https://github.com/argv0/nbds) - C implementations of several scalable non-blocking data structures for x86 and x86-64.
* [armon/libart](https://github.com/armon/libart) - Adaptive Radix Trees implemented in C
* [arnimarj/py-pointless](https://github.com/arnimarj/py-pointless) - A fast and efficient read-only relocatable data structure for JSON like data, with C and Python APIs
* [ashinkarov/trie](https://github.com/ashinkarov/trie) - Simple implementation of trie data structure in C
* [bcopeland/em_misc](https://github.com/bcopeland/em_misc) - external memory data structure playground
* [begeekmyfriend/bplustree](https://github.com/begeekmyfriend/bplustree) - A minimal but extreme fast B+ tree indexing structure demo for billions of key-value storage
* [bpudream/pat](https://github.com/bpudream/pat) - Data Structure (中国大学MOOC-陈越、何钦铭-数据结构)
* [breckinloggins/ngtemplate](https://github.com/breckinloggins/ngtemplate) - ngtemplate - A template engine written in C designed to be syntax-compatible with Google CTemplate
* [cengek/CKDatastruct](https://github.com/cengek/CKDatastruct) - The using of data structure in C from our class
* [cbgbt/DataStructures](https://github.com/cbgbt/DataStructures) - A data structures library written in C.
* [chrismoos/hash-ring](https://github.com/chrismoos/hash-ring) - C hash ring library
* [chriso/bitset](https://github.com/chriso/bitset) - A compressed bitset with supporting data structures and algorithms
* [chucknthem/Data-structures-algorithms](https://github.com/chucknthem/Data-structures-algorithms) - Collection of Data structures, algorithms and interesting bits of code.
* [clibs/list](https://github.com/clibs/list) - C doubly linked list
* [codeprepper/data-structures](https://github.com/codeprepper/data-structures) - arrays, linked lists, stacks and queues
* [coderaven/B-Tree](https://github.com/coderaven/B-Tree) - B-Tree Implementation in C. A project in Data Structures.
* [corks/corc.ds](https://github.com/corks/corc.ds) - A data structure library written in C.
* [cstavish/c_data_structs](https://github.com/cstavish/c_data_structs) - singly/doubly linked list and hash table implementations...more to come
* [davidar/c-hashtable](https://github.com/davidar/c-hashtable) - Git mirror of the hash table data structure in C by Christopher Clark
* [dhbikoff/Generic-C-Library](https://github.com/dhbikoff/Generic-C-Library) - A library of generic data structures in C
* [dgvncsz0f/lift](https://github.com/dgvncsz0f/lift) - Implementation of some data structures in C
* [dminor/skip-quadtree](https://github.com/dminor/skip-quadtree) - Implementation of the skip quadtree and compressed quadtree data structures.
* [douglascrockford/DEC64](https://github.com/douglascrockford/DEC64) - Decimal floating point
* [esheldon/meds](https://github.com/esheldon/meds) - Python and C libraries to work with Multi Epoch Data Structures
* [fmela/libdict](https://github.com/fmela/libdict) - C library of key-value data structures with an object-oriented interface.
* [fragglet/c-algorithms](https://github.com/fragglet/c-algorithms) - A library of common data structures and algorithms written in C.
* [freels/ruby_trie](https://github.com/freels/ruby_trie) - Native C implementation of a trie data structure.
* [fritz0705/libf](https://github.com/fritz0705/libf) - Library to make programming simpler and cleaner (and slower, because I was too lazy to implement usable data structures)
* [fubarwrangler/datastruct](https://github.com/fubarwrangler/datastruct) - A silly project to code some data structures to help brush up on my C
* [ghostrong/algorithm](https://github.com/ghostrong/algorithm) - Data Structure and Algorithms
* [gnudennis/ds_c](https://github.com/gnudennis/ds_c) - Data Structure In C
* [graphitemaster/libintrusive](https://github.com/graphitemaster/libintrusive) - Intrusive data structures for C
* [grundprinzip/bitcompressedvector](https://github.com/grundprinzip/bitcompressedvector) - Provide a container for integral data types that applies light-weight bit compression
* [hacatu/haclib](https://github.com/hacatu/haclib) - A utility library providing data types C should have been made with such as vectors and sequences, mostly as macros.
* [harnold/generic-c](https://github.com/harnold/generic-c) - A library of generic data structures and algorithms for C, in the spirit of the STL
* [hyPiRion/c-rrb](https://github.com/hyPiRion/c-rrb) - RRB-tree implemented as a library in C.
* [hyPiRion/persistencia](https://github.com/hyPiRion/persistencia) - Repository with implementations to understand persistent data structures.
* [hyPiRion/roulette-tree](https://github.com/hyPiRion/roulette-tree) - Data structure for efficient fitness-proportionate selection.
* [igorsobreira/iclib](https://github.com/igorsobreira/iclib) - Library with useful C data structures
* [jaimz/core_ds](https://github.com/jaimz/core_ds) - Simple C data structure library
* [jarun/dslib](https://github.com/jarun/dslib) - A library of handy data structures
* [johnj/llds](https://github.com/johnj/llds) - Low-Level Data Structure - efficient data structures, and fast data access in the 2.6/3.0 kernel
* [joshdk/libmap](https://github.com/joshdk/libmap) - A map (data structure) library written in c
* [jtsiomb/kdtree](https://github.com/jtsiomb/kdtree) - A simple C library for working with KD-Trees
* [jsvennevid/filearchive](https://github.com/jsvennevid/filearchive) - File archive library allowing for easy creation and access to data stored inside a container through a simple API.
* [jvirkki/libbloom](https://github.com/jvirkki/libbloom) - A simple and small bloom filter implementation in plain C.
* [ksheedlo/kmdata](https://github.com/ksheedlo/kmdata) - Data structures for C programmers, by C programmers.
* [louiswins/RB-Tree](https://github.com/louiswins/RB-Tree) - An implementation of the Red-Black Tree data structure.
* [livioso/datastructures-in-C](https://github.com/livioso/datastructures-in-C) - Implementation of a some data structures in C for educational purposes. For example featuring a trie implementation in C (inspired by DAS84 "a bit of C") or a XOR linked list.
* [malbrain/Btree-source-code](https://github.com/malbrain/Btree-source-code) - A working project for High-concurrency B-tree source code in C
* [marekweb/datastructs-c](https://github.com/marekweb/datastructs-c) - Arraylist and Hashtable implementation in C
* [michaeltyson/TPCircularBuffer](https://github.com/michaeltyson/TPCircularBuffer) - A simple, fast circular buffer implementation
* [mikedlowis/data-structures](https://github.com/mikedlowis/data-structures) - A collection of data structures implemented in C to be included in multiple projects.
* [mrnugget/data_structures](https://github.com/mrnugget/data_structures) - Implementations of common data structures in C
* [naraing/dsLib](https://github.com/naraing/dsLib) - An algorithm library with core data-sttructures and common algortihm implementations on those data structures
* [natehardison/data-structures](https://github.com/natehardison/data-structures) - A bunch of data structure implementations, just for fun.
* [noporpoise/BitArray](https://github.com/noporpoise/BitArray) - C bit array structs and methods
* [noporpoise/madcrowlib](https://github.com/noporpoise/madcrowlib) - Common C data structure macros
* [orangejulius/cs_fundamentals](https://github.com/orangejulius/cs_fundamentals) - simple implementations of common data structures/algorithms
* [paulasmuth/libsmatrix](https://github.com/paulasmuth/libsmatrix) - thread-safe sparse matrix data structure
* [pcdavid/data-structures](https://github.com/pcdavid/data-structures) - Sample implementations of classical data structures in C.
* [pcostesi/c-data-structures](https://github.com/pcostesi/c-data-structures) - Simple Data Structures
* [petewarden/c_hashmap](https://github.com/petewarden/c_hashmap) - A simple string hashmap in C
* [pforemski/libpjf](https://github.com/pforemski/libpjf) - A C library of data structures with tools (based on libasn)

## Events ##
* [libuv][397] - Cross-platform asynchronous I/O. [``MIT``][MIT]
* [libPhenom][398] - Eventing framework for building high-scalability and
  high-performance systems. [``Apache-2.0``][Apache-2.0]
* [libev][399] - Yet another event loop. [``BSD-2-Clause``][BSD-2-Clause]
* [libevent][400] - Event loop replacement for network servers. [``BSD-3-Clause``][BSD-3-Clause]
* [Lupus/libevfibers](https://github.com/Lupus/libevfibers) - Small C fiber library that uses libev based event loop and libcoro based coroutine context switching.
* [facebook/libphenom](https://github.com/facebook/libphenom) - An eventing framework for building high performance and high scalability systems in C.
* [joyent/libuv](https://github.com/joyent/libuv) - Go to
* [libuv/libuv](https://github.com/libuv/libuv) - Cross-platform asychronous I/O
* [nmathewson/Libevent](https://github.com/nmathewson/Libevent) - Nick's public libevent repository.  The official repository is at         git://levent.git.sourceforge.net/gitroot/levent/libevent

## FFI ##
Foreign function interfaces, also know as binding interfaces.
* [libffi][404] - Portable foreign-function interface library. [``MIT``][MIT]
* [GNU Libffcall][405] - Collection of libraries for building foreign function
  interfaces. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [dyncall][406] - Another foreign function interface library. [``MIT``][MIT]
* [atgreen/libffi](https://github.com/atgreen/libffi) - A portable foreign-function interface library.
* [dyu/ffi-overhead](https://github.com/dyu/ffi-overhead) - comparing the c ffi (foreign function interface) overhead on various programming languages
* [jmckaskill/luaffi](https://github.com/jmckaskill/luaffi) - Standalone FFI library for calling C functions from lua. Compatible with the luajit FFI interface.

## Flow Control and Language Extension ##
* [libCello][429] - Library introducing higher-level programming to C. [``BSD-3-Clause``][BSD-3-Clause]
* [Ragel][430] - DSL for state machines that compiles to C. [``GPL-2.0-only``][GPL-2.0-only]
* [Kitsune][431] - Efficient, general-purpose framework for dynamic software
  updating. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [yasm](http://yasm.tortall.net/) - Yasm Modular Assembler Project. [`2-clause BSD`](https://directory.fsf.org/wiki/License:BSD-2-Clause)
* [P99](http://p99.gforge.inria.fr/) - Suite of macros to implement advanced features like default function arguments, scope-bound resources, etc. (Requires C99) [`Q Public License`](https://tldrlegal.com/license/q-public-license-1.0-(qpl-1.0)#summary)
* [orangeduck/Cello](https://github.com/orangeduck/Cello) - Higher level programming in C
* [CObjectSystem/COS](https://github.com/CObjectSystem/COS) - C Object System
* [H2CO3/Sparkling](https://github.com/H2CO3/Sparkling) - Lightweight extension language
* [LuaDist/lua](https://github.com/LuaDist/lua) - The Lua programming language with CMake based build
* [LuaDist/luajit](https://github.com/LuaDist/luajit) - LuaJIT is JIT compiler for the Lua language.
* [LuaDist/toluapp](https://github.com/LuaDist/toluapp) - tolua++ is an extension of toLua, a tool to integrate C/Cpp code with Lua
* [Zeex/subhook](https://github.com/Zeex/subhook) - Simple hooking library for C/C++ (x86 only, 32/64-bit, no dependencies)
* [alexanderchuranov/Metaresc](https://github.com/alexanderchuranov/Metaresc) - META data and RESource library for  C language
* [arnaudbrejeon/cspec](https://github.com/arnaudbrejeon/cspec) - Behavior driven development in C
* [cioc/functionalC](https://github.com/cioc/functionalC) - Not because it is good, but because we can...
* [comex/substitute](https://github.com/comex/substitute) - A free runtime modification library.
* [elua/elua](https://github.com/elua/elua) - eLua Project on GitHub
* [eudoxia0/magma](https://github.com/eudoxia0/magma) - Extending C with cmacro
* [graphitemaster/lambdapp](https://github.com/graphitemaster/lambdapp) - Anonymous functions in C
* [guillermocalvo/exceptions4c](https://github.com/guillermocalvo/exceptions4c) - :bomb: An exception handling framework for C
* [orangeduck/LuaAutoC](https://github.com/orangeduck/LuaAutoC) - Automagically use C Functions and Structs with the Lua API
* [pfultz2/Cloak](https://github.com/pfultz2/Cloak) - A mini-preprocessor library to demostrate the recursive capabilites of the preprocessor

## Game Development ##
Engines, libraries and other helpful things specifically for making games.
* [Allegro][170] - Cross-platform, game development and multimedia library. [``Zlib``][Zlib]
* [cglm][171] - Optimized OpenGL/Graphics Math (glm) for C. [``MIT``][MIT]
* [Chipmunk2D][172] - Fast and lightweight 2D game physics library. [``MIT``][MIT]
* [Corange][173] - Game engine in pure C. [``BSD-2-Clause``][BSD-2-Clause]
* [CSFML][174] - Binding for [SFML][175]. [``Zlib``][Zlib]
* [Darkplaces][176] - Modified version of the Quake2 engine. [``GPL-2.0-only``][GPL-2.0-only]
* [Epoxy][177] - Library for handling OpenGL function pointer management. [``MIT``][MIT]
* [Freecell Solver][178] - Set of libraries and command-line programs for
  automatically solving FreeCell and some similar variants of card Solitaire. [``MIT``][MIT]
* [ioquake3][181] - Quake3 engine, freed at last. [``GPL-2.0-only``][GPL-2.0-only]
* [kazmath][182] - Maths library for games. [``BSD-2-Clause``][BSD-2-Clause]
* [libao][183] - Cross-platform audio library with a wide variety of outputs. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [MATHC][184] - Math library for 2D and 3D programming. [``ZLib``][Zlib]
* [Orx][185] - Portable, lightweight, plugin-based, data-driven, 2D-oriented
  game engine. [``Zlib``][Zlib]
* [Quake][186] - Quake engine. [``GPL-2.0-only``][GPL-2.0-only]
* [Quake2][187] - Quake2 engine. [``GPL-2.0-only``][GPL-2.0-only]
* [raylib][188] - Simple library to learn video game programming. [``Zlib``][Zlib]
* [RetroArch][189] - Reference frontend for [libretro][190]. [``GPL-3.0-only``][GPL-3.0-only]
* [SDL2][191] - Cross-platform library designed to provide low-level access to
  audio, keyboard, mouse, joystick and graphics hardware via OpenGL. [``Zlib``][Zlib]
* [sdl-gpu][192] - Library for high-performance, modern 2D graphics. Based on
  SDL. [``MIT``][MIT]
* [SIGIL][193] - Sound, Input and Graphics Integration Library; a simple
  alternative to other libraries for doing all those things. Various licenses,
  all open source.
* [Spearmint][194] - Engine designed for FPS games. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Corange](https://github.com/orangeduck/Corange) - Game engine in pure C. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [Darkplaces](https://icculus.org/twilight/darkplaces/) - Modified version of the Quake2 engine. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [ioquake3](https://ioquake3.org/) - The Quake3 engine, freed at last. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [Orx](http://orx-project.org/) - Portable, lightweight, plugin-based, data-driven, 2D-oriented game engine. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [Quake](https://github.com/id-Software/Quake) - The Quake engine. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [Quake2](https://github.com/id-Software/Quake-2) - The Quake2 engine. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [Spearmint](https://clover.moe/spearmint/) - Engine designed for FPS games. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [Allegro](https://liballeg.org/) - Cross-platform, video game development and multimedia library. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [Chipmunk2D](http://chipmunk-physics.net/) - Fast and lightweight 2D game physics library. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [CSFML](https://www.sfml-dev.org/download/csfml/) - Binding for [SFML](https://www.sfml-dev.org/index.php) in C. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [FreeGLUT](http://freeglut.sourceforge.net/) - Alternative to the OpenGL Utility Toolkit. Allows the creation and management of windows with OpenGL contexts. [`X11`](https://directory.fsf.org/wiki/License:X11)
* [GLFW](https://www.glfw.org/) - Multi-platform library for creating windows with OpenGL contexts. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [libao](https://xiph.org/ao/) - Cross-platform audio library with a wide variety of outputs. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [RetroArch](https://www.libretro.com/) - The reference frontend for [libretro](https://www.libretro.com/). [`GNU GPL3`](http://www.gnu.org/licenses/gpl.html)
* [SDL and SDL2](https://www.libsdl.org/) - Cross-platform development library designed to provide low-level access to audio, keyboard, mouse, joystick and graphics hardware via OpenGL. SDL2 is the most current version. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [raylib](https://www.raylib.com/) - Simple and easy-to-use library to learn videogames programming. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [Gigoteur/UnicornConsole](https://github.com/Gigoteur/UnicornConsole) - Unicorn Console: create quick game !
* [HBehrens/obj2opengl](https://github.com/HBehrens/obj2opengl) - script to convert 3D models of OBJ files to C/C++ float arrays (vertices, faces, texture) compatible with OpenGL ES glDrawArrays compatible with iPhone/iPad
* [HerculesWS/Hercules](https://github.com/HerculesWS/Hercules) - Hercules is a collaborative software development project revolving around the creation of a robust massively multiplayer online role playing game (MMORPG) server package. Written in C, the program is very versatile and provides NPCs, warps and modifications. The project is jointly managed by a group of volunteers located around the world as well as a tremendous community providing QA and support. Hercules is a continuation of the original Athena project.
* [Kazade/kazmath](https://github.com/Kazade/kazmath) - A C math library targeted at games
* [MarilynDafa/Bulllord-Engine](https://github.com/MarilynDafa/Bulllord-Engine) - lightspeed lightweight elegant  game engine in pure c
* [MauriceGit/Cloth_Simulation](https://github.com/MauriceGit/Cloth_Simulation) - Cloth-Visualization via particle-simulation.
* [MauriceGit/Partikel_accelleration_on_GPU](https://github.com/MauriceGit/Partikel_accelleration_on_GPU) - Particle accelleration with OpenGL 4.3, using the compute shader to calculate particle movement on graphics hardware.
* [Olde-Skuul/doom3do](https://github.com/Olde-Skuul/doom3do) - The complete archive for DOOM for the 3DO
* [R4stl1n/cAudio](https://github.com/R4stl1n/cAudio) - 3D Audio Engine Based on Openal
* [RandyGaul/AsciiEngine](https://github.com/RandyGaul/AsciiEngine) - Game engine written in C to create Ascii art games within the Windows console.
* [Tangent128/luasdl2](https://github.com/Tangent128/luasdl2) - A pure C binding of SDL 2.0 for Lua 5.1, Lua 5.2, and LuaJIT.
* [a-nikolaev/curseofwar](https://github.com/a-nikolaev/curseofwar) - A Real Time Strategy game for Linux.
* [ands/lightmapper](https://github.com/ands/lightmapper) - A C/C++ single-file library for drop-in lightmap baking. Just use your existing OpenGL renderer to bounce light!
* [ands/seamoptimizer](https://github.com/ands/seamoptimizer) - A C/C++ single-file library that minimizes the hard transition errors of disjoint edges in lightmaps.
* [cadwallion/spinel](https://github.com/cadwallion/spinel) - A free and open source game engine using mruby and C/C++
* [ccore/ccore](https://github.com/ccore/ccore) - A cross platform low level game development library
* [ccore/ccore_rewrite](https://github.com/ccore/ccore_rewrite) - A cross platform low level game development library
* [chocolate-doom/chocolate-doom](https://github.com/chocolate-doom/chocolate-doom) - Chocolate Doom is a Doom source port that is minimalist and historically accurate.
* [cloudwu/skynet](https://github.com/cloudwu/skynet) - A lightweight online game framework
* [cocos2d/cocos2d-frame](https://github.com/cocos2d/cocos2d-frame) - Player and "stub" for cocos2d
* [cxong/cdogs-sdl](https://github.com/cxong/cdogs-sdl) - Classic overhead run-and-gun game
* [dalerank/caesaria-game](https://github.com/dalerank/caesaria-game) - Caesar III (Open source remake)
* [dariomanesku/cmft](https://github.com/dariomanesku/cmft) - Cross-platform open-source command-line cubemap filtering tool.
* [ebassi/graphene](https://github.com/ebassi/graphene) - A thin layer of graphic data types
* [eduard-permyakov/permafrost-engine](https://github.com/eduard-permyakov/permafrost-engine) - An OpenGL 3.3 RTS game engine written in C
* [ejoy/ejoy2d](https://github.com/ejoy/ejoy2d) - A 2D Graphics Engine for Mobile Game
* [etlegacy/etlegacy](https://github.com/etlegacy/etlegacy) - ET: Legacy is based on the source code of the Wolfenstein: Enemy Territory which was released under the GPLv3 license. The main goal of this project is to fix bugs, remove old dependencies and make it playable on all major operating systems while still remaining compatible with the ET 2.60b version and as many of its mods as possible.
* [fabiensanglard/chocolate_duke3D](https://github.com/fabiensanglard/chocolate_duke3D) - chocolate Duke Nukem,3D
* [felselva/mathc](https://github.com/felselva/mathc) - Pure C math library for 2D and 3D programming.
* [floooh/chips](https://github.com/floooh/chips) - 8-bit chip and system emulators in standalone C headers
* [fogleman/Craft](https://github.com/fogleman/Craft) - A simple Minecraft clone written in C using modern OpenGL (shaders).
* [gabomdq/SDL_GameControllerDB](https://github.com/gabomdq/SDL_GameControllerDB) - A community sourced database of game controller mappings to be used with SDL2 Game Controller functionality
* [geon/gloss](https://github.com/geon/gloss) - A bidirectional path tracer written in C.
* [id-Software/DOOM](https://github.com/id-Software/DOOM) - DOOM Open Source Release
* [id-Software/Quake-2](https://github.com/id-Software/Quake-2) - Quake 2 GPL Source Release
* [id-Software/Quake-III-Arena](https://github.com/id-Software/Quake-III-Arena) - Quake III Arena GPL Source Release
* [id-Software/Quake](https://github.com/id-Software/Quake) - Quake GPL Source Release
* [jarikomppa/soloud](https://github.com/jarikomppa/soloud) - Free, easy, portable audio engine for games
* [keendreams/keen](https://github.com/keendreams/keen) - Keen Dreams on Greenlight!
* [libgdx/fbx-conv](https://github.com/libgdx/fbx-conv) - Command line utility using the FBX SDK to convert FBX/Collada/Obj files to a custom text/binary format for static, keyframed and skinned meshes.
* [liballeg/allegro5](https://github.com/liballeg/allegro5) - The official Allegro 5 git repository. Pull requests welcome!
* [linleyh/liberation-circuit](https://github.com/linleyh/liberation-circuit) - Trapped in a hostile computer system, you must make a way out - RTS/coding game
* [mainroach/crabby](https://github.com/mainroach/crabby) - A texture compression algorithm for sprite sheets that allows decompression on the GPU during rendering.
* [martincohen/Punity](https://github.com/martincohen/Punity) - A tiny game engine in C.
* [mupen64plus/mupen64plus-core](https://github.com/mupen64plus/mupen64plus-core) - Core module of the Mupen64Plus project
* [naev/naev](https://github.com/naev/naev) - Naev is a 2d action/rpg space game that combines elements from the action, rpg and simulation genres.
* [nikki93/cgame](https://github.com/nikki93/cgame) - some ideas involving games and C
* [orangeduck/Corange](https://github.com/orangeduck/Corange) - Pure C Game Engine

## Graphics ##
Access to graphical APIs or other graphic rendering libraries.
* [FreeGLUT][179] - Alternative to the OpenGL Utility Toolkit. Allows the
  creation and management of windows with OpenGL contexts. [``X11``][X11]
* [GLFW][180] - Multi-platform library for creating windows with OpenGL
  contexts. [``Zlib``][Zlib]
* [Cairo][196] - 2D graphics library. [``LGPL-2.1-only``][LGPL-2.1-only] or [``MPL-1.1``][205]
* [graphene][197] - Thin layer of graphical data types. [``MIT``][MIT]
* [libcaca][198] - ASCII renderer for terminal-based interfaces. [``WTFPL``][WTFPL]
* [libsixel][199] - Library implementing the SIXEL protocol, allowing beautiful
  graphics in your terminal. [``MIT``][MIT]
* [libxmi][200] - Function library for rasterizing 2D vector
  graphics. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [lightmapper][201] - Single-file library for lightmap baking, using an
  existing OpenGL renderer. Public domain.
* [nanovg][202] - Anti-aliased 2D vector drawing library on top of OpenGL, for
  UI and visualizations. [``Zlib``][Zlib]
* [OpenGL][203] - Industry standard for high-performance graphics, with a
  native C binding. [Various licenses][204].
* [OpenGL](https://www.opengl.org/) - Industry adopted 2D and 3D graphics API. More resources at [awesome-opengl](https://github.com/eug/awesome-opengl).
* [OpenGL ES](https://www.khronos.org/opengles/) - Industry adopted 2D and 3D graphics API for mobile and embedded devices.
* [OpenGL SC](https://www.khronos.org/openglsc/) - Graphic and compute standard for industry requiring system safety certification.
* [Vulkan](https://www.khronos.org/vulkan/) - Explicit graphic and compute API for modern cross-platform development. More resources at [awesome-vulkan](https://github.com/vinjn/awesome-vulkan).
* [Cairo](https://www.cairographics.org/) -2D graphics library. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`MPLv1.1`](https://directory.fsf.org/wiki/License:MPL-1.1)
* [Cogl](https://github.com/rib/cogl-web/wiki) - GPU graphics and utilities API. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [Clutter](https://blogs.gnome.org/clutter/get-it/) - UI library based on OpenGL. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [glfw/glfw](https://github.com/glfw/glfw) - A multi-platform library for OpenGL, OpenGL ES, Vulkan, window and input
* [nigels-com/glew](https://github.com/nigels-com/glew) - The OpenGL Extension Wrangler Library
* [anoek/ex-sdl-cairo-freetype-harfbuzz](https://github.com/anoek/ex-sdl-cairo-freetype-harfbuzz) - Example code which uses SDL, cairo, freetype, and harfbuzz to do ttf/otf text layout and rendering
* [ashima/webgl-noise](https://github.com/ashima/webgl-noise) - Procedural Noise Shader Routines compatible with WebGL
* [blodow/realtime_urdf_filter](https://github.com/blodow/realtime_urdf_filter) - ROS package that can filter geometry defined in URDF models from Kinect depth images. Can also preprocess data for the OpenNI tracker, to remove backgrounds, robots etc.
* [grz0zrg/fbg](https://github.com/grz0zrg/fbg) - Lightweight C 2D graphics API agnostic library with parallelism support
* [grimfang4/sdl-gpu](https://github.com/grimfang4/sdl-gpu) - A library for high-performance, modern 2D graphics with SDL written in C.
* [ileben/ShivaVG](https://github.com/ileben/ShivaVG) - OpenGL based ANSI C implementation of the OpenVG standard.
* [jpbruyere/vkvg](https://github.com/jpbruyere/vkvg) - Vulkan vector drawing, try to stay close to cairo api
* [libretro/common-shaders](https://github.com/libretro/common-shaders) - Collection of commonly used Cg shaders. These shaders are usable by either HLSL and/or Cg runtime compilers. The cg2glsl script will translate most of these into GLSL shaders.
* [memononen/nanovg](https://github.com/memononen/nanovg) - Antialiased 2D vector drawing library on top of OpenGL for UI and visualizations.
* [micahpearlman/MonkVG](https://github.com/micahpearlman/MonkVG) - MonkVG is an OpenVG 1.1 like vector graphics API implementation optimized for game use currently using an OpenGL ES backend that should be compatible with any HW that supports OpenGL ES 2.0 which includes most iOS and Android devices.
* [minusinf/opengl_dataviewer](https://github.com/minusinf/opengl_dataviewer) - A simple OpenGL xyzw dataviewer

## GUI ##
* [GTK+][206] - Cross-platform widget toolkit. [``LGPL-2.1-only``][LGPL-2.1-only]
* [IUP][207] - Another cross-platform widget toolkit. [``MIT``][MIT]
* [nuklear][208] - Small, C89, single-header widget toolkit. Public domain.
* [tinyfiledialogs][209] - Single-file library for simple dialogs. Compatible
  with many other toolkits and OSes. [``Zlib``][Zlib]
* [Tk][210] - Basic widget toolkit. Part of Tcl/Tk. [``TCL``][TCL]
* [XForms Toolkit][211] - Widget toolkit designed for the XWindow system. [``LGPL-2.1-only``][LGPL-2.1-only]
* [Glade][415] - RAD tool to enable quick development of GTK+ GUIs. [``GPL-2.0-only``][GPL-2.0-only]
* [vurtun/nuklear](https://github.com/vurtun/nuklear) - A single-header ANSI C gui library
* [andlabs/libui](https://github.com/andlabs/libui) - Simple and portable (but not inflexible) GUI library in C that uses the native GUI technologies of each platform it supports.
* [lc-soft/LCUI](https://github.com/lc-soft/LCUI) - A small C library for building user interfaces with C, XML and CSS.
* [littlevgl/lvgl](https://github.com/littlevgl/lvgl) - Graphics library to create an embedded GUI with easy-to-use graphical elements, beautiful visual effects and low memory footprint. It offers anti-aliasing, opacity, and animations using only one frame buffer.
* [ocornut/imgui_club](https://github.com/ocornut/imgui_club) - Nice things to use along dear imgui

## Hardware Oriented ##
* [libusb][407] - Provides generic access to USB devices. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libimobiledevice][408] - Cross-platform protocol library to communicate
  with iThings. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [cpu\_features][409] - Get CPU features at runtime. [``Apache-2.0``][Apache-2.0]
* [libcoap][423] - Implementation of the [Constrained Application Protocol][424].
  [``GPL-2.0-or-later``][GPL-2.0-or-later] or [``BSD-2-Clause``][BSD-2-Clause]
* [libnfc][438] - Platform-independent Near-Field Communication library. [``LGPL-3.0-only``][LGPL-3.0-only]
* [GTK+](https://www.gtk.org/) - Cross-platform widget toolkit. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [IUP](http://webserver2.tecgraf.puc-rio.br/iup/) - Another cross-platform widget toolkit. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [Tk](http://www.tcl.tk/) - Basic widget toolkit. Part of Tcl/Tk. [`Tcl/Tk License`](http://www.tcl.tk/software/tcltk/license.html)
* [XForms Toolkit](http://xforms-toolkit.org/) - Widget toolkit designed for the XWindow system. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [nuklear](https://github.com/vurtun/nuklear) - Single-header ANSI C gui library. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [libui](https://github.com/andlabs/libui) - Simple and portable (but not inflexible) GUI library. [`MIT`](https://github.com/andlabs/libui/blob/master/LICENSE)
* [LCUI](https://github.com/lc-soft/LCUI/) - Small C library for building user interfaces with C, XML and CSS. [`MIT`](https://github.com/lc-soft/LCUI/blob/develop/LICENSE.TXT)
* [Genymobile/scrcpy](https://github.com/Genymobile/scrcpy) - Display and control your Android device
* [AdysTech/raspy-weather](https://github.com/AdysTech/raspy-weather) - A set of C libraries to gather Temperature and Humidity data from generic DHT11 sensor, store it in a round-robin database and show it in a PHP page.
* [Azure/azure-iot-sdk-c](https://github.com/Azure/azure-iot-sdk-c) - A C99 SDK for connecting devices to Microsoft Azure IoT services
* [Eugnis/spectre-attack](https://github.com/Eugnis/spectre-attack) - Example of using revealed "Spectre" exploit (CVE-2017-5753 and CVE-2017-5715)
* [FoxelSA/libfastcal](https://github.com/FoxelSA/libfastcal) - Fast calibration data access
* [OpenSC/OpenSC](https://github.com/OpenSC/OpenSC) - Open source smart card tools and middleware. PKCS#11/MiniDriver/Tokend
* [OpenSecurityResearch/iclass_dump](https://github.com/OpenSecurityResearch/iclass_dump) - Tools to pull data from HID iClass readers
* [Stephane-D/SGDK](https://github.com/Stephane-D/SGDK) - SGDK: A small, open and free development kit for the Sega Megadrive
* [alonbl/pkcs11-data](https://github.com/alonbl/pkcs11-data) - PKCS#11 data object manipulator
* [andygock/avr-uart](https://github.com/andygock/avr-uart) - AVR UART C Library
* [anrieff/libcpuid](https://github.com/anrieff/libcpuid) - a small C library for x86 CPU detection and feature extraction
* [coocox/cox](https://github.com/coocox/cox) - CoX is an peripherals library with a unified standard interface specially for ARM Cortex M.
* [edorfaus/TEMPered](https://github.com/edorfaus/TEMPered) - C library and program for reading the TEMPer family of thermometer and hygrometer devices.
* [google/cpu_features](https://github.com/google/cpu_features) - A cross platform C99 library to get cpu features at runtime.
* [jackmitch/libsoc](https://github.com/jackmitch/libsoc) - libsoc: C library for interfacing with common SoC peripherals through generic kernel interfaces
* [joan2937/pigpio](https://github.com/joan2937/pigpio) - pigpio is a C library for the Raspberry which allows control of the General Purpose Input Outputs (GPIO).
* [leaflabs/libmaple](https://github.com/leaflabs/libmaple) - [INACTIVE] C and C++ library for STM32 ARM Cortex-M3 development boards.
* [libimobiledevice/libimobiledevice](https://github.com/libimobiledevice/libimobiledevice) - A cross-platform protocol library to communicate with iOS devices
* [libopencm3/libopencm3](https://github.com/libopencm3/libopencm3) - Open Source ARM cortex m microcontroller library
* [libusb/libusb](https://github.com/libusb/libusb) - A cross-platform library to access USB devices
* [micronucleus/micronucleus](https://github.com/micronucleus/micronucleus) - ATTiny usb bootloader with a strong emphasis on bootloader compactness.
* [nfc-tools/libnfc](https://github.com/nfc-tools/libnfc) - Platform independent Near Field Communication (NFC) library
* [openyou/libomron](https://github.com/openyou/libomron) - Libraries for accessing data from Omron medical devices

## Hashing ##
Hash function implementations for *non*-crypto purposes. Cryptographic hashes
can be found in the Crypto section.
* [CLHash][165] - Library implementing fast CLHash hashing function. Only works
  on Intel Haswell or newer. [``Apache-2.0``][Apache-2.0]
* [HighwayHash][166] - Fast, strong, SIMD-using hash function. Also contains an
  implementation of SipHash. [``Apache-2.0``][Apache-2.0]
* [SpookyHash][167] - Fast hash function. [``BSD-3-Clause``][BSD-3-Clause]
* [t1ha][168] - Fast Positive Hash - a portable, fast hash function. [``BSD-3-Clause``][BSD-3-Clause]
* [xxHash][169] - Fast 32 and 64 bit hashing algorithm. [``BSD-2-Clause``][BSD-2-Clause]
* [GNU gperf][414] - Perfect hash function generator, given a list of strings.
  Outputs C code. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [jwHash](https://github.com/watmough/jwHash) - Fast hashtable implementation. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [xxHash](http://cyan4973.github.io/xxHash/) - Extremely fast non-cryptographic hash algorithm. [`2-clause BSD`](https://directory.fsf.org/wiki/License:BSD-2-Clause)
* [libcrc](https://github.com/PeterScott/murmur3) - Multi platform CRC library. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [murmur](https://github.com/ispc/ispc) - C implementation of MurMur Hashing. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [Cyan4973/xxHash](https://github.com/Cyan4973/xxHash) - Extremely fast non-cryptographic hash algorithm
* [PeterScott/murmur3](https://github.com/PeterScott/murmur3) - Murmur3 hash in C
* [RJ/ketama](https://github.com/RJ/ketama) - C library for consistent hashing, and langauge bindings
* [begeekmyfriend/CuckooFilter](https://github.com/begeekmyfriend/CuckooFilter) - Substitute for bloom filter.
* [bitly/dablooms](https://github.com/bitly/dablooms) - scaling, counting, bloom filter library
* [clibs/hash](https://github.com/clibs/hash) - C hash implementation based on khash
* [cr-marcstevens/sha1collisiondetection](https://github.com/cr-marcstevens/sha1collisiondetection) - Library and command line tool to detect SHA-1 collision in a file
* [lemire/clhash](https://github.com/lemire/clhash) - C library implementing the ridiculously fast CLHash  hashing function
* [mattsta/crcspeed](https://github.com/mattsta/crcspeed) - This make CRC be fast.  Included implementations: CRC-64-Jones and CRC-16-CCITT

## Image Processing and Computer Vision ##
* [ccv][5] - C-based/Cached/Core Computer Vision library; modern computer
  vision. [``BSD-3-Clause``][BSD-3-Clause]
* [libgd][380] - Library for the dynamic creation of images by programmers. [``MIT``][MIT]
* [giflib][381] - Library for reading and writing gif images. [``MIT``][MIT]
* [libimagequant][383] - Small, portable library for high-quality conversion of
  RGBA images to 8-bit indexed colour images. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libjpeg-turbo][384] - Faster library for reading and writing JPEG files. [Various licences][194]
* [libpng][385] - Official PNG reference library. [``Libpng``][Libpng]
* [libRSVG][386] - Library to render SVG files using Cairo. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libvips][387] - Image processing library. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [mozjpeg][388] - Improved JPEG encoder. [``BSD-3-Clause``][BSD-3-Clause]
* [lodepng][389] - Simple PNG image decoder and encoder, requiring no other
  dependencies. [``BSD-3-Clause``][BSD-3-Clause]
* [libimagequant](https://pngquant.org/lib/) - Small, portable library for high-quality conversion of RGBA images to 8-bit indexed colour images. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [libjpeg-turbo](https://libjpeg-turbo.org/) - Faster library for reading and writing JPEG files. [`Various Licenses`](https://libjpeg-turbo.org/About/License)
* [libpng](http://www.libpng.org) - The official PNG reference library. [`libpng license`](http://www.libpng.org/pub/png/src/libpng-LICENSE.txt)
* [libxmi](https://www.gnu.org/software/libxmi/) - Function library for rasterizing 2D vector graphics. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [mozjpeg](https://github.com/mozilla/mozjpeg) - Improved JPEG encoder. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libccv](http://libccv.org) - Modern Computer Vision Library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [liuliu/ccv](https://github.com/liuliu/ccv) - C-based/Cached/Core Computer Vision Library, A Modern Computer Vision Library
* [MartinMittring/dcraw_exif](https://github.com/MartinMittring/dcraw_exif) - dcraw (Camera RAW format processor) from Dave Coffin with updates, additionally maintain exif data for using it with Agisoft PhotoScan
* [Phildo/pixQL](https://github.com/Phildo/pixQL) - SQL for image processing
* [XadillaX/byakuren](https://github.com/XadillaX/byakuren) - 🎭 A theme color extracting library implemented by C.
* [ansilove/AnsiLove-C](https://github.com/ansilove/AnsiLove-C) - ANSi / ASCII art to PNG converter in C
* [ansilove/ansilove](https://github.com/ansilove/ansilove) - ANSi / ASCII art to PNG converter in C
* [bluesmoon/pngtocss](https://github.com/bluesmoon/pngtocss) - Read in a gradient from a png file and spit out CSS for it
* [brendangregg/Dump2PNG](https://github.com/brendangregg/Dump2PNG) - Visualize file data as a PNG
* [buaazp/zimg](https://github.com/buaazp/zimg) - A lightweight and high performance image storage and processing system.
* [dbohdan/s2png](https://github.com/dbohdan/s2png) - Store data of any kind inside PNG images.
* [derekmolloy/boneCV](https://github.com/derekmolloy/boneCV) - Beaglebone Webcam and OpenCV Examples Repository
* [ginsweater/gif-h](https://github.com/ginsweater/gif-h) - Simple C++ one-header library for the creation of animated GIFs from image data.
* [jcupitt/libvips](https://github.com/jcupitt/libvips) - A fast image processing library with low memory needs.
* [mozilla/mozjpeg](https://github.com/mozilla/mozjpeg) - Improved JPEG encoder.
* [openslide/openslide](https://github.com/openslide/openslide) - C library for reading virtual slide images

## Integrated Debugging and Logging ##
* [whereami][390] - One-file library for locating the current executable on the
  file system. [``WTFPL``][WTFPL]
* [zlog][391] - Reliable, pure C logging library. [``LGPL-2.1-only``][LGPL-2.1-only]
* [debug][392] - One-header library for easier 'printf debugging'. [``MIT``][MIT]
* [CException][393] - Implementation of exceptions. [``MIT``][MIT]
* [pblog](https://github.com/google/pblog) - Small, low overhead, structured logging library intended for logging formware events.[`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [0xmalloc/c-log](https://github.com/0xmalloc/c-log) - a fast ,stable and thread-safe log lib(logger) for C/C++ language
* [Celtoys/Remotery](https://github.com/Celtoys/Remotery) - Single C file, Realtime CPU/GPU Profiler with Remote Web Viewer
* [HardySimpson/zlog](https://github.com/HardySimpson/zlog) - A reliable, high-performance, thread safe, flexsible, clear-model, pure C logging library.
* [armink/CmBacktrace](https://github.com/armink/CmBacktrace) - Advanced fault backtrace library for ARM Cortex-M series MCU | ARM Cortex-M 系列 MCU 错误追踪库
* [armink/EasyLogger](https://github.com/armink/EasyLogger) - A ultra-lightweight(ROM<1.6K, RAM<0.3k), high-performance C/C++ log library. | 一款超轻量级(ROM<1.6K, RAM<0.3k)、高性能的 C/C++ 日志库
* [cyrus-and/prof](https://github.com/cyrus-and/prof) - Self-contained C/C++ profiler library for Linux
* [esneider/debug](https://github.com/esneider/debug) - Debugging like a sir (in C)
* [facebook/liblogfaf](https://github.com/facebook/liblogfaf) - A library that logs messages using non-blocking UDP datagrams.
* [kmcallister/embedded-breakpoints](https://github.com/kmcallister/embedded-breakpoints) - Embed GDB breakpoints in C source code
* [ntpeters/SimpleLogger](https://github.com/ntpeters/SimpleLogger) - Basic logger for C and C++ projects
* [openjudge/sandbox](https://github.com/openjudge/sandbox) - The sandbox libraries (libsandbox & pysandbox) are an open-source suite of software components for C/C++ and Python developers to create automated profiling tools and watchdog programs. The API's are designed for executing and instrumenting simple (single process) tasks, featuring policy-based behavioral auditing, resource quota, and statistics collecting.

## Lexing and Parsing ##
Generic lexers and parsers
* [flex][356] - Fast lexical analyzer generator. [``BSD-2-Clause``][BSD-2-Clause]
* [GNU Bison][357] - General-purpose parser generator that converts an
  annotated context-free grammar into a range of parsers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [hammer][358] - Parser combinators for binary formats. [``GPL-2.0-only``][GPL-2.0-only]
* [mpc][359] - Parser combinator library. [``BSD-2-Clause``][BSD-2-Clause]
* [re2c][360] - Lexer generator, producing fast lexers, with access to its
  internals. Public domain.
* [MatzeB/cparser](https://github.com/MatzeB/cparser) - C99 parser and frontend for libfirm
* [XVilka/cparse](https://github.com/XVilka/cparse) - Parser of C-syntax data definitions, C-syntax function definitions
* [bbu/simple-interpreter](https://github.com/bbu/simple-interpreter) - A hackable and extensible lexer, parser and interpreter for a minimalistic, imperative, C-like language.
* [burtonsamograd/sxc](https://github.com/burtonsamograd/sxc) - sxc is an 'S-Expression C' transpiler for generating C code using macros written in Common Lisp
* [dcreager/libpush](https://github.com/dcreager/libpush) - An arrow-based parser combinator library for C
* [kmussel/Moment](https://github.com/kmussel/Moment) - Natural Language Date Parser Using Lex/Yacc/C
* [orangeduck/mpc](https://github.com/orangeduck/mpc) - A Parser Combinator library for C

## Memory Management ##
* [Boehm GC][212] - Garbage collection for C. Various licenses, all open source.
* [jemalloc][213] - Malloc implementation that emphasizes avoidance of
  fragmentation and scalable concurrency support. [``BSD-2-Clause``][BSD-2-Clause]
* [Lockless Memory Allocator][214] - Efficient memory allocator. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [rpmalloc][215] - Thread-caching, fast memory allocator, naturally aligned on
  32-byte boundaries. Public domain.
* [talloc][216] - Hierarchical, reference-counted memory pool system with
  destructors. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [tlsf][217] - Two-Level Segregated Fit allocator; a general-purpose, dynamic
  memory allocator designed to meet real-time requirements.
  [Up-to-date implementation][218]. [``BSD-3-Clause``][BSD-3-Clause]
* [jemalloc](http://jemalloc.net/) - General purpose malloc(3) implementation that emphasizes fragmentation avoidance and scalable concurrency support, commonly used in production systems. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [dlmalloc](http://g.oswego.edu/pub/misc/malloc.c) - Doug Lea's malloc(3) implementation, useful for academic and research purposes. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [Hoard](http://hoard.org/) - A Fast, Scalable, and Memory-efficient Malloc for Linux, Windows, Mac, and Solaris. [`GNU GPL2`](http://www.gnu.org/licenses/gpl.html)
* [nedmalloc](http://www.nedprod.com/programs/portable/nedmalloc/) - An EXTREMELY FAST portable thread caching malloc(3) implementation written in C. [`GNU GPL2`](http://www.gnu.org/licenses/gpl.html)
* [rpmalloc](https://github.com/rampantpixels/rpmalloc) - Cross platform, lock-free memory allocator. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [CCareaga/heap_allocator](https://github.com/CCareaga/heap_allocator) - A simple heap memory allocator in ~200 lines.
* [ivmai/bdwgc](https://github.com/ivmai/bdwgc) - The Boehm-Demers-Weiser conservative C/C++ Garbage Collector (libgc, bdwgc, boehm-gc)
* [mulle-nat/mulle-allocator](https://github.com/mulle-nat/mulle-allocator) - 🔄 Flexible C memory allocation scheme with leak checking
* [munificent/mark-sweep](https://github.com/munificent/mark-sweep) - A simple mark-sweep garbage collector in C
* [ned14/nedmalloc](https://github.com/ned14/nedmalloc) - An EXTREMELY FAST portable thread caching malloc implementation written in C for multiple threads without lock contention based on dlmalloc. Optimised for x86 and x64. Compatible with C++. Can patch itself into existing binaries on Windows.
* [orangeduck/tgc](https://github.com/orangeduck/tgc) - A Tiny Garbage Collector for C

## Multimedia ##
Audio and video processing
* [ApeTagLibs][428] - Library for working with APEv2 tags. [``MIT``][MIT]
* [aubio][219] - Library for audio and music analysis. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [FFMPEG][220] - Complete, cross-platform solution to record, convert and
  stream audio and video. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [GStreamer][221] - Framework for audio and visual media. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libmpv][222] - Music-playing library. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [libsndfile][223] - Library for reading and writing sound files. Supports
  many formats. [``LGPL-2.1-only``][LGPL-2.1-only] or [``LGPL-3.0-only``][LGPL-3.0-only]
* [libsoundio][224] - Library for cross-platform, real-time audio input and
  output. Has a range of back-ends. [``MIT``][MIT]
* [minimp3][225] - Lightweight MP3 decoder single header library. [``CC0-1.0``][CC0-1.0]
* [Soundpipe][226] - Lightweight music DSP library. [``MIT``][MIT]
* [FFMPEG](https://www.ffmpeg.org/) - Complete, cross-platform solution to record, convert and stream audio and video. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`GNU GPL2.1 or later (some parts)`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [GStreamer](https://gstreamer.freedesktop.org/) - Framework for audio and visual media. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [lodepng](https://lodev.org/lodepng/) - Simple PNG image decoder and encoder, requiring no other dependencies. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libsoup](https://wiki.gnome.org/action/show/Projects/libsoup?action=show&redirect=LibSoup) - GNOME HTTP client/server library. Uses GObject. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libmpv](https://mpv.io/) - Music-playing library. Compile with ``./waf configure --disable-cplayer --enable-libmpv-shared`` to not have the music player. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [libsoundio](http://libsound.io/) - Library for cross-platform, real-time audio input and output. Has a range of back-ends. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [AVbin/AVbin](https://github.com/AVbin/AVbin) - AVbin is a C library that provides a thin, cross-platform wrapper around Libav’s video- and audio-decoding functionality, providing long-term binary compatibility for applications and languages that need it.  See also: Pyglet, a python media framework that makes extensive use of AVbin.
* [LnxPrgr3/crossfeed](https://github.com/LnxPrgr3/crossfeed) - Headphone crossfeed filter
* [PaulBatchelor/Soundpipe](https://github.com/PaulBatchelor/Soundpipe) - A lightweight music DSP library.
* [Themaister/libfmsynth](https://github.com/Themaister/libfmsynth) - A C library which implements an FM synthesizer
* [UniversalPrimer/flv-analyzer](https://github.com/UniversalPrimer/flv-analyzer) - Loads an FLV file into sane C data structures and outputs fields as human readable
* [Vidvox/hap-qt-codec](https://github.com/Vidvox/hap-qt-codec) - A QuickTime codec for Hap video
* [acrisci/playerctl](https://github.com/acrisci/playerctl) - 🎧 mpris command-line controller and library for spotify, vlc, audacious, bmp, cmus, and others.
* [andrewrk/libsoundio](https://github.com/andrewrk/libsoundio) - C library for cross-platform real-time audio input and output
* [aubio/aubio](https://github.com/aubio/aubio) - a library for audio and music analysis
* [cmatsuoka/libxmp](https://github.com/cmatsuoka/libxmp) - Libxmp is a library that renders module files to PCM data.
* [cnlohr/colorchord](https://github.com/cnlohr/colorchord) - Chromatic Sound to Light Conversion System
* [csound/csound](https://github.com/csound/csound) - Main repository for Csound
* [dxjia/ffmpeg-commands-executor-library](https://github.com/dxjia/ffmpeg-commands-executor-library) - execute ffmpeg commands through a jni shared library.
* [erikd/libsndfile](https://github.com/erikd/libsndfile) - A C library for reading and writing sound files containing sampled audio data..
* [imankulov/wav2rtp](https://github.com/imankulov/wav2rtp) - wav2rtp is a simple tool intended to convert speech data from wav files to RTP data stream
* [kfish/libfishsound](https://github.com/kfish/libfishsound) - A simple programming interface for decoding and encoding audio data using Xiph.org codecs (FLAC, Speex and Vorbis)
* [libass/libass](https://github.com/libass/libass) - libass is a portable subtitle renderer for the ASS/SSA (Advanced Substation Alpha/Substation Alpha) subtitle format.
* [libav/libav](https://github.com/libav/libav) - Libav github mirror, clone of git://git.libav.org/libav
* [libpd/libpd](https://github.com/libpd/libpd) - Pure Data embeddable audio synthesis library
* [mltframework/mlt](https://github.com/mltframework/mlt) - MLT Multimedia Framework

## Multiple Purpose Libraries ##
* [pal][65] - Optimized library for maths, parallel processing and data
  movement. [``Apache-2.0``][Apache-2.0]
* [APR][154] - Apache Portable Runtime; another library of cross-platform
  utility functions. [``Apache-2.0``][Apache-2.0]
* [C Algorithms][155] - Collection of common algorithms and data structures. [``ISC``][ISC]
* [CPL][156] - The Common Pipeline Library; a set of libraries designed to be a
  comprehensive, efficient and robust software toolkit. [``GPL-2.0-only``][GPL-2.0-only]
* [EFL][157] - Large collection of useful data structures and functions. Various
  licenses, all open source.
* [klib][158] - Small and lightweight implementations of common algorithms and
  data structures. [``MIT``][MIT]
* [libcork][159] - Utility functions and structures, designed for
  resource-constrained systems. Can be embedded. [``BSD-3-Clause``][BSD-3-Clause]
* [libnih][160] - Lightweight library of functions and structures. [``GPL-2.0-only``][GPL-2.0-only]
* [libU][161] - Small library of basic utilities, including memory allocation,
  string manipulation and logging. [``BSD-3-Clause``][BSD-3-Clause]
* [PBL][162] - Large library of utilities, featuring data structures, among
  other things. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [qlibc][163] - Simple and powerful library, designed as a replacement for GLib
  while focusing on being small and light. [``BSD-2-Clause``][BSD-2-Clause]
* [TBOX][164] - Multi-platform library with a large number of capabilities. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [gnulib][425] - Collection of common GNU code. Various licenses, all
  open source.
* [APR](http://apr.apache.org/) - Apache Portable Runtime; another library of cross-platform utility functions. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [C Algorithms](https://fragglet.github.io/c-algorithms/) - Collection of common algorithms and data structures for C. [`ISC`](https://directory.fsf.org/wiki/License:ISC)
* [CPL](http://www.eso.org/sci/software/cpl/) - The Common Pipeline Library; a set of libraries designed to be a comprehensive, efficient and robust software toolkit. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [EFL](https://www.enlightenment.org/) - Large collection of useful data structures and functions.
* [GLib](https://wiki.gnome.org/Projects/GLib) - Library of utility functions and structures, designed to be portable, efficient and powerful. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [GIO](https://developer.gnome.org/gio/) - Modern and easy-to-use VFS API. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [GObject](https://developer.gnome.org/gobject/stable/) - Object-oriented system and object model for C. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libnih](https://github.com/keybuk/libnih) - Lightweight library of C functions and structures. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [libU](http://www.koanlogic.com/libu/) - Small library of basic utilities, including memory allocation, string manipulation and logging. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [PBL](http://www.mission-base.com/peter/source/) - Large library of utilities, featuring data structures, among other things. [`GNU LGPL2.1 or later (library)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`GNU GPL2.1 or later (test code)`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [qlibc](http://wolkykim.github.io/qlibc/) - Simple and powerful C library, designed as a replacement for GLib while focusing on being small and light. [`qLib license`](https://github.com/wolkykim/qlibc/blob/master/LICENSE) (similar to [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD))
* [stb](https://github.com/nothings/stb) - Range of single-file libraries for C. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [libsrt](https://faragon.github.io/libsrt.html) - Safe Real-Time library for C. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [chutsu/cog](https://github.com/chutsu/cog) - C common library containing common data structures, sorting algorithms and utility functions
* [cs50/libcs50](https://github.com/cs50/libcs50) - CS50 Library for C
* [dcreager/libcork](https://github.com/dcreager/libcork) - A simple, easily embeddable cross-platform C library
* [faragon/libsrt](https://github.com/faragon/libsrt) - libsrt is a C library for writing fast and safe C code, faster. It provides string, vector, bit set, set, map, hash set, and hash map handling. Suitable for soft and hard real-time. Allows both heap and stack allocation.  *BETA* (API still can change: suggestions are welcome)
* [gregvirgin/libcork](https://github.com/gregvirgin/libcork) - A simple, easily embeddable cross-platform C library
* [happyfish100/libfastcommon](https://github.com/happyfish100/libfastcommon) - c common functions library extracted from my open source project FastDFS. this library is very simple and stable.  functions including: string, logger, chain, hash, socket, ini file reader, base64 encode / decode, url encode / decode, fast timer, skiplist, object pool etc. detail info please see the c header files.
* [koanlogic/libu](https://github.com/koanlogic/libu) - LibU is a multiplatform utility library written in C, with APIs for handling memory allocation, networking and URI parsing, string manipulation, debugging, and logging in a very compact way, plus many other miscellaneous tasks
* [letoram/arcan](https://github.com/letoram/arcan) - Arcan - [Display Server, Multimedia Framework, Game Engine] -> "Desktop Engine"

## Networking ##
### DNS ###
* [GNU adns][229] - Advanced, easy-to-use, asynch-capable DNS client library
  and utilities. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [ldns][231] - Library to simplify DNS programming. [``BSD-3-Clause``][BSD-3-Clause]
* [bagder/c-ares](https://github.com/bagder/c-ares) - c-ares is a C library for asynchronous DNS requests
* [farsightsec/dnstable](https://github.com/farsightsec/dnstable) - encoding format, library, and utilities for passive DNS data

### HTTP ###
* [http-parser][230] - HTTP request/response parser. [``MIT``][MIT]
* [libsagui][239] - Library for cross-platform HTTP servers. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [lwan][242] - Experimental, scalable, high-performance HTTP server. [``GPL-2.0-only``][GPL-2.0-only]
* [mongoose][243] - Embedded web server. [``GPL-2.0-only``][GPL-2.0-only]
* [libhttpd][234] - Library to add basic web server capabilities to an
  application or embedded device. [``GPL-2.0-only``][GPL-2.0-only]
* [libmicrohttpd][236] - Small library that makes it easy to run an HTTP
  server as part of another application. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libonion][237] - HTTP server library, designed to be easy to use. [``Apache-2.0``][Apache-2.0]
* [nodejs/http-parser](https://github.com/nodejs/http-parser) - http request/response parser for c
* [civetweb/civetweb](https://github.com/civetweb/civetweb) - Embedded C/C++ web server
* [h2o/h2o](https://github.com/h2o/h2o) - H2O - the optimized HTTP/1, HTTP/2 server
* [h2o/picohttpparser](https://github.com/h2o/picohttpparser) - tiny HTTP parser written in C (used in HTTP::Parser::XS et al.)
* [iafonov/multipart-parser-c](https://github.com/iafonov/multipart-parser-c) - Http multipart parser implemented in C
* [joyent/http-parser](https://github.com/joyent/http-parser) - http request/response parser for c
* [zyearn/zaver](https://github.com/zyearn/zaver) - Yet another fast and efficient HTTP server
* [monkey/monkey](https://github.com/monkey/monkey) - Monkey HTTP Server

### Mail ###
* [LibEtPan][233] - Mail library providing an efficient network for IMAP, SMTP,
  POP and NNTP. [``BSD-3-Clause``][BSD-3-Clause]
* [libvldmail][439] - Email validation library. No external dependencies
  (not even regexps). [``WTFPL``][WTFPL]
* [libquickmail][238] - Library intended to give developers a way to send email
  from their applications. Supports multiple To/Cc/Bcc recipients and
  attachments without size limits. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [dinhviethoa/libetpan](https://github.com/dinhviethoa/libetpan) - Mail Framework for C Language

### Messaging ###
* [NNG][245] - nanomsg-next-generation - lightweight brokerless messaging. [``MIT``][MIT]
* [rabbitmq-c][440] - Client library for [RabbitMQ][229]. [``MIT``][MIT]
* [zproto][370] - Protocol framework for ZeroMQ. [``MIT``][MIT]
* [nanomsg][244] - C-based implementation of ZeroMQ. [``MIT``][MIT]
* [antirez/disque](https://github.com/antirez/disque) - Disque is a distributed message broker
* [circonus-labs/fq](https://github.com/circonus-labs/fq) - F@#$*&%Q (Message queue that is fast, brokered, in C and gets out of your way)
* [paulasmuth/fyrehose](https://github.com/paulasmuth/fyrehose) - message broker for JSON data streams

### Other Networking ###
* [asnlc][227] - Compiler of ASN.1 specifications into C source code. [``BSD-2-Clause``][BSD-2-Clause]
* [CHL][228] - C Hypertext Library - A library for writing for web in C. [``GPL-3.0-only``][GPL-3.0-only]
* [libcurl][232] - Client-side URL transfer library, supporting a wide range of
  formats. [``curl``][curl]
* [libidn][235] - Implementation of the Stringprep, Punycode and IDNA
  specifications. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [LibVNCServer][240] - Cross-platform libraries to implement VNC server and/or
  client functionality. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [oSip][246] - SIP implementation without additional dependencies. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [socket99][247] - C99 wrapper for the BSD sockets API. [``ISC``][ISC]
* [zyre][249] - Framework for proximity-based peer-to-peer applications. [``MPL-2.0``][MPL-2.0]
* [libgss][435] - Generic Security Service. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [asnlc](http://lionet.info/asn1c/compiler.html) - Compiler of ASN.1 specifications into C source code. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [czmq](http://czmq.zeromq.org/) - High-level binding for ZeroMQ. [`MPL2.0`](https://www.gnu.org/licenses/license-list.html#MPL-2.0)
* [GNU adns](https://www.gnu.org/software/adns/) - Advanced, easy-to-use, asynch-capable DNS client library and utilities. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GNU SASL](https://www.gnu.org/software/gsasl/) - Implementation of the Simple Authentication and Security Layer and a few common SASL mechanism. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GnuTLS](https://www.gnutls.org/) - Secure communication library, implementing SSL, TLS and DTLS. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [gumbo-parser](https://github.com/google/gumbo-parser) - HTML5 parsing library in C99. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [http-parser](https://github.com/nodejs/http-parser) - HTTP request/response parser. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [ldns](https://www.nlnetlabs.nl/projects/ldns/index.html) - Library to simplify DNS programming. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libcurl](https://curl.haxx.se/libcurl/) - Client-side URL transfer library, supporting a wide range of formats. [`curl license`](https://curl.haxx.se/docs/copyright.html)
* [LibEtPan](http://www.etpan.org/) - Mail library providing an efficient network for IMAP, SMTP, POP and NNTP. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libev](http://software.schmorp.de/pkg/libev.html) - Yet another event loop. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [libuv](http://libuv.org/) - Cross-platform asynchronous I/O. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libevent](http://libevent.org/) - Event loop replacement for network servers. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libgss](https://www.gnu.org/software/gss/) - Generic Security Service. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [libhttpd](http://www.hughes.com.au/products/libhttpd/) - Library to add basic web server capabilities to an application or embedded device. [`GNU GPL2`](http://www.gnu.org/licenses/gpl.html)
* [libidn](https://www.gnu.org/software/libidn/) - Implementation of the Stringprep, Punycode and IDNA specifications. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [libmicrohttpd](https://www.gnu.org/software/libmicrohttpd/) - Small C library that makes it easy to run an HTTP server as part of another application. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libsagui](https://risoflora.github.io/libsagui/) - Sagui is a cross-platform C library which helps to develop web servers or frameworks. [`GNU LGPL3`](http://www.gnu.org/licenses/lgpl.html)
* [libvldmail](https://github.com/dertuxmalwieder/libvldmail) - Your friendly e-mail address validation library. [`WTFPLv2`](http://www.wtfpl.net/txt/copying/)
* [lwan](https://lwan.ws/) - Experimental, scalable, high-performance HTTP server. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [mongoose](https://cesanta.com/) - Embedded web server for C. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [MQTT-C](https://github.com/LiamBindle/MQTT-C) - Portable MQTT C client for embedded systems and PCs alike. [`MIT`](https://raw.githubusercontent.com/LiamBindle/MQTT-C/master/LICENSE)
* [nanomsg](https://github.com/nanomsg/nanomsg) - C-based implementation of ZeroMQ. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [oSip](https://www.gnu.org/software/osip/) - SIP implementation in C without additional dependencies. [`GNU LGPLv2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [pig](https://github.com/rafael-santiago/pig) - Linux packet crafting tool. [`GPL2`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [s2n](https://github.com/awslabs/s2n) - C99 implementation of the TLS/SSL protocols, designed to be simple, fast and with security as a priority. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [socket99](https://github.com/silentbicycle/socket99) - C99 wrapper for the BSD sockets API. [`ISC`](https://directory.fsf.org/wiki/License:ISC)
* [Tox](https://tox.chat/) - Communication platform, designed to be a Skype-killer. [`GNU GPL3`](http://www.gnu.org/licenses/gpl.html)
* [librg](https://github.com/librg/librg) - Library for building simple and elegant cross-platform mmo client-server solutions. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [dyad](https://github.com/rxi/dyad) - Asynchronous networking library. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [h2o](https://github.com/h2o/h2o/) - Optimized HTTP/1, HTTP/2 high performance server/library. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [51Degrees/Device-Detection](https://github.com/51Degrees/Device-Detection) - THE Fastest and most Accurate device detection for C / PHP / Perl / Python and Node.js - professionally maintained device data
* [uriparser](https://uriparser.github.io) - Strictly RFC 3986-compliant URI parsing and handling library. [``BSD-3-Clause``][BSD-3-Clause]
* [ElementsProject/lightning](https://github.com/ElementsProject/lightning) - c-lightning — a Lightning Network implementation in C
* [FreeRDP/FreeRDP](https://github.com/FreeRDP/FreeRDP) - FreeRDP is a free remote desktop protocol library and clients
* [FreeRDP/Remmina](https://github.com/FreeRDP/Remmina) - The GTK+ Remmina Remote Desktop Client
* [GROX13/BitTorrent](https://github.com/GROX13/BitTorrent) - BitTorrent is a protocol for the practice of peer-to-peer file sharing that is used to distribute large amounts of data over the Internet. BitTorrent is one of the most common protocols for transferring large files, and peer-to-peer networks have been estimated to collectively account for approximately 43% to 70% of all Internet traffic (depending on geographical location) as of February 2009. In November 2004, BitTorrent was responsible for 35% of all Internet traffic. As of February 2013, BitTorrent was responsible for 3.35% of all worldwide bandwidth, more than half of the 6% of total bandwidth dedicated to file sharing.
* [JFreegman/toxic](https://github.com/JFreegman/toxic) - An ncurses-based Tox client
* [LibVNC/libvncserver](https://github.com/LibVNC/libvncserver) - LibVNCServer/LibVNCClient are cross-platform C libraries that allow you to easily implement VNC server or client functionality in your program.
* [Librevault/librevault](https://github.com/Librevault/librevault) - Librevault - Peer-to-peer, decentralized and open source file sync.
* [Netsukuku/netsukuku](https://github.com/Netsukuku/netsukuku) - Revived C-code
* [Tox/toxic](https://github.com/Tox/toxic) - CLI Tox client
* [armon/bloomd](https://github.com/armon/bloomd) - C network daemon for bloom filters
* [armon/hlld](https://github.com/armon/hlld) - C network daemon for HyperLogLogs
* [bagder/spindly](https://github.com/bagder/spindly) - a portable C library for SPDY transport (DEAD project!)
* [boazsegev/c-server-tools](https://github.com/boazsegev/c-server-tools) - Write network services in C using dynamic protocols such as HTTP and Websockets
* [c9s/r3](https://github.com/c9s/r3) - libr3 is a high-performance path dispatching library. It compiles your route paths into a prefix tree (trie). By using the constructed prefix trie in the start-up time, you may dispatch your routes with efficiency
* [cesanta/fossa](https://github.com/cesanta/fossa) - Async non-blocking multi-protocol networking library for C/C++
* [chmduquesne/xmppipe](https://github.com/chmduquesne/xmppipe) - This program allows to pipe data through an xmpp tunnel
* [chokepoint/CryptHook](https://github.com/chokepoint/CryptHook) - TCP/UDP symmetric encryption tunnel wrapper
* [clibs/dumpasn1](https://github.com/clibs/dumpasn1) - Display the contents of ASN.1 encoded data
* [deltachat/deltachat-core](https://github.com/deltachat/deltachat-core) - Delta.Chat C-Library with e2e chat-over-email functionality & Python bindings
* [fastos/fastsocket](https://github.com/fastos/fastsocket) - Fastsocket is a highly scalable socket and its underlying networking implementation of Linux kernel. With the straight linear scalability, Fastsocket can provide extremely good performance in multicore machines. In addition, it is very easy to use and maintain. As a result, it has been deployed in the production environment of SINA.
* [felipec/msn-pecan](https://github.com/felipec/msn-pecan) - MSN Messenger library in C
* [iem-projects/pd-iemrtp](https://github.com/iem-projects/pd-iemrtp) - RTP support for Pure Data
* [igraph/igraph](https://github.com/igraph/igraph) - Library for the analysis of networks
* [irungentoo/toxcore](https://github.com/irungentoo/toxcore) - The future of online communications.
* [japeq/bencode-tools](https://github.com/japeq/bencode-tools) - bencode-tools is a collection of tools for manipulating bencoded data.
* [libssh2/libssh2](https://github.com/libssh2/libssh2) - the SSH library
* [lsalzman/enet](https://github.com/lsalzman/enet) - ENet reliable UDP networking library
* [mopemope/meinheld](https://github.com/mopemope/meinheld) - meinheld is a high performance asynchronous WSGI Web Server (based on picoev)
* [nanomsg/nanomsg](https://github.com/nanomsg/nanomsg) - nanomsg library
* [neilalexander/sigmavpn](https://github.com/neilalexander/sigmavpn) - Light-weight, secure and modular VPN solution which makes use of NaCl encryption (also available for Android using jnacl in "sigmavpn-android")
* [neutrinolabs/xrdp](https://github.com/neutrinolabs/xrdp) - xrdp: an open source RDP server
* [nicolasff/river](https://github.com/nicolasff/river) - A simple “comet” server in C, streaming data to web clients
* [obgm/libcoap](https://github.com/obgm/libcoap) - A CoAP (RFC 7252) implementation in C
* [opendp/dpdk-odp](https://github.com/opendp/dpdk-odp) - Open data plane on dpdk, TCP/IP stack for dpdk.

### Websockets ###
* [Wslay][248] - WebSocket library. Implements version 13 of the WebSocket
  protocol, as described in RFC 6455. [``MIT``][MIT]
* [libwebsock][241] - Easy-to-use and powerful web socket library. [``LGPL-3.0-only``][LGPL-3.0-only]
* [m8rge/cwebsocket](https://github.com/m8rge/cwebsocket) - cWebsocket is lightweight websocket server library
* [payden/libwebsock](https://github.com/payden/libwebsock) - C library for easy WebSockets server.

--------------------------------------------------------------------------------

## OS Specifics ##
* [attr][401] - Commands for manipulating filesystem extended attributes. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [Caffeine][402] - Library for building daemons and services for Linux and
  FreeBSD systems. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libcox][403] - Library which permits cross-platform system calls and
  standard utilities across different operating systems. [``BSD-2-Clause``][BSD-2-Clause]
* [GNU FreeIPMI][422] - In-band and out-of-band IPMI implementation. [``GPL-3.0-only``][GPL-3.0-only]
* [CRIU][427] - Checkpoint/Restore In Userspace; a software tool (with a C API)
  for 'freezing' a running application to disk, then restoring it. Targeted for
  Linux. [``GPL-2.0-only``][GPL-2.0-only] or [``LGPL-2.1-only``][LGPL-2.1-only]
* [linenoise][433] - Small, self-contained alternative to readline and libedit. [``BSD-2-Clause``][BSD-2-Clause]
* [alsa-lib](http://www.alsa-project.org/main/index.php/Main_Page) - Userspace library to interact with ALSA. [`LGPL2.1`](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
* [Leandros/WindowsHModular](https://github.com/Leandros/WindowsHModular) - A modular Windows.h Header. Licensed under Public Domain & MIT.
* [Microsoft/Windows-driver-samples](https://github.com/Microsoft/Windows-driver-samples) - This repo contains driver samples prepared for use with Microsoft Visual Studio and the Windows Driver Kit (WDK). It contains both Universal Windows Driver and desktop-only driver samples.
* [Microsoft/checkedc](https://github.com/Microsoft/checkedc) - Checked C is an extension to C that adds checking to detect or prevent common programming errors such as buffer overruns and out-of-bounds memory accesses.  This repo has a wiki for Checked C, sample code, the specification, and test code.
* [Xfennec/progress](https://github.com/Xfennec/progress) - Linux tool to show progress for cp, rm, dd, ...
* [a0rtega/pafish](https://github.com/a0rtega/pafish) - Pafish is a demonstration tool that employs several techniques to detect sandboxes and analysis environments in the same way as malware families do.
* [adoxa/ansicon](https://github.com/adoxa/ansicon) - Process ANSI escape sequences for Windows console programs.
* [aidenbell/getdents](https://github.com/aidenbell/getdents) - Simple tool for listing large (millions) numbers of files on Linux systems without causing memory issues. Useful for shell scripting large data stores.
* [antirez/linenoise](https://github.com/antirez/linenoise) - A small self-contained alternative to readline and libedit
* [ardagnir/athame](https://github.com/ardagnir/athame) - Full vim for readline (bash, gdb, python, etc)
* [asamy/ksm](https://github.com/asamy/ksm) - A really simple and lightweight x64 hypervisor written in C.  Supports VMFUNC, EPTP switching, #VE EPT Violation, VT-x nesting and IDT shadowing.  VMFUNC backward compatibility also supported.
* [dtrace4linux/linux](https://github.com/dtrace4linux/linux) - dtrace for linux - kernel driver and userland tools
* [fancycode/MemoryModule](https://github.com/fancycode/MemoryModule) - Library to load a DLL from memory.
* [gentilkiwi/kekeo](https://github.com/gentilkiwi/kekeo) - A little toolbox to play with Microsoft Kerberos in C
* [jimon/osx_app_in_plain_c](https://github.com/jimon/osx_app_in_plain_c) - A simple showcase how to create a simple OS X app in plain C without any Objective-C
* [martinezjavier/ldd3](https://github.com/martinezjavier/ldd3) - Linux Device Drivers 3 examples updated to work in recent kernels

## Procedural Generation ##
* [heman][382] - Tiny library of image utilities dealing with height maps,
  normal maps, distance fields and the like. [``MIT``][MIT]
* [JCash/voronoi](https://github.com/JCash/voronoi) - A C implementation for creating 2D voronoi diagrams

## Regex and Search ##
* [Onigmo][275] - Fork of Oniguruma, supporting more advanced regexps. [``BSD-2-Clause``][BSD-2-Clause]
* [Oniguruma][276] - Regex library supporting a wide range of encodings, and
  incorporating many security-oriented fixes. [``BSD-2-Clause``][BSD-2-Clause]
* [PCRE][277] - Implementation of regexes identical to that of Perl 5. [``BSD-3-Clause``][BSD-3-Clause]
* [SLRE][278] - Super Light Regular Expression library; a small implementation
  of a subset of Perl regex syntax. [``GPL-2.0-only``][GPL-2.0-only]
* [TRE][279] - POSIX-compliant, feature-full regex library. [``BSD-2-Clause``][BSD-2-Clause]
* [PCRE](http://www.pcre.org/) - Implementation of regexes identical to that of Perl 5. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [regexp4](https://github.com/nasciiboy/recursiveregexpraptor-4) - Simple and complete implementation of regular expressions with its own sintax. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [SLRE](https://github.com/cesanta/slre) - Super Light Regular Expression library; a very small implementation of a subset of Perl regex syntax. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [TRE](https://github.com/laurikari/tre/) - POSIX-compliant, feature-full regex library. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [sregex](https://github.com/openresty/sregex) - Non-backtracking NFA/DFA-based Perl-compatible regex engine library. [`3-clause BSD`](https://opensource.org/licenses/BSD-3-Clause)
* [JazzCore/ctrlp-cmatcher](https://github.com/JazzCore/ctrlp-cmatcher) - CtrlP C matching extension
* [Maxime2/dataparksearch](https://github.com/Maxime2/dataparksearch) - An open source, feature rich search engine.
* [cesanta/slre](https://github.com/cesanta/slre) - Super Light Regexp engine for C/C++
* [k-takata/Onigmo](https://github.com/k-takata/Onigmo) - Onigmo is a regular expressions library forked from Oniguruma.
* [kkos/oniguruma](https://github.com/kkos/oniguruma) - regular expression library
* [mbornet-hl/hl](https://github.com/mbornet-hl/hl) - Highlight (colorize) text data using regular expressions
* [mptre/pick](https://github.com/mptre/pick) - A fuzzy search tool for the command-line
* [openresty/sregex](https://github.com/openresty/sregex) - A non-backtracking NFA/DFA-based Perl-compatible regex engine matching on large data streams

## Serialization ##
* [binn][280] - Binary serialization format, meant to be compact, fast and
  easy-to-use. [``Apache-2.0``][Apache-2.0]
* [c-capnproto][281] - Implementation of the Cap'n Proto serialization protocol. [``MIT``][MIT]
* [cmp][282] - Implementation of the [MessagePack][283] serialization protocol. [``MIT``][MIT]
* [flatcc][284] - [FlatBuffers][285] compiler and library. [``Apache-2.0``][Apache-2.0]
* [libavro][286] - Implementation of the Avro data serialization system. [``Apache-2.0``][Apache-2.0]
* [mpack][287] - Another implementation of the [MessagePack][283] serialization
  protocol. [``MIT``][MIT]
* [OPIC][288] - Object Persistence in C; a revolutionary serialization
  framework, with matching on-disk and in-memory representations. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [protobuf-c][289] - Implementation of Google Protocol Buffer. [``BSD-2-Clause``][BSD-2-Clause]
* [tpl][290] - Small binary serialization library. [``MIT``][MIT]
* [xdr][291] - External Data Representation; a standard for data serialization.
  Standard (no license applicable).
* [pbc][437] - Protocol buffers library. [``MIT``][MIT]
* [binn](https://github.com/liteserver/binn) - Binary serialization format meant to be compact, fast and easy-to-use. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [c-capnproto](https://github.com/jmckaskill/c-capnproto) - Implementation of the Cap'n Proto serialization protocol. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [cmp](https://github.com/camgunz/cmp) - Implementation of the [MessagePack](https://msgpack.org/) serialization protocol. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libavro](http://avro.apache.org/docs/current/api/c/index.html#_introduction_to_avro_c) - C implementation of the Avro data serialization system. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [mpack](https://github.com/ludocode/mpack) - Another implementation of the [MessagePack](https://msgpack.org/) serialization protocol. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [netstring-c](https://github.com/liteserver/netstring-c) - Netstring encoder and decoder. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [protobuf-c](https://github.com/protobuf-c/protobuf-c) - Implementation of Google Protocol Buffer in C. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [xdr](https://en.wikipedia.org/wiki/External_Data_Representation) - External Data Representation; a standard for data serialization.
* [ErikDubbelboer/c-pack](https://github.com/ErikDubbelboer/c-pack) - Simple data packing/unpacking in C
* [Xsoda/struct](https://github.com/Xsoda/struct) - pack and unpack packet data like python struct module.
* [acg/lwpb](https://github.com/acg/lwpb) - Lightweight Protocol Buffers for C and Python
* [camgunz/cmp](https://github.com/camgunz/cmp) - An implementation of the MessagePack serialization format in C / msgpack.org[C]
* [cloudwu/atomdict](https://github.com/cloudwu/atomdict) - A data structure for data exchange between multi lua states.
* [cloudwu/pbc](https://github.com/cloudwu/pbc) - A protocol buffers library for C
* [cloudwu/sproto](https://github.com/cloudwu/sproto) - Yet another protocol library like google protocol buffers , but simple and fast.
* [dryman/opic](https://github.com/dryman/opic) - Fast serialization framework for C
* [fredrikbk/libpack](https://github.com/fredrikbk/libpack) - Library that packs/serializes or unpacks/deserializes user-defined data layouts. The data layouts are specified using datatypes similar to MPI Datatypes. The library compiles the datatypes into efficient vectorized pack/unpack code at commit time using an LLVM-based online compiler.
* [google/upb](https://github.com/google/upb) - a small protobuf implementation in C
* [greghaynes/Afproto](https://github.com/greghaynes/Afproto) - Serial data framing protocol
* [ludocode/mpack](https://github.com/ludocode/mpack) - MPack - A C encoder/decoder for the MessagePack serialization format / msgpack.org[C]
* [nanopb/nanopb](https://github.com/nanopb/nanopb) - Protocol Buffers with small code size

## Source Code Collections ##
* [CCAN][292] - Modelled after Perl's CPAN, this is a big collection of code.
  Various licenses, all open source.
* [clib][293] - Something of a package manager. Comes with a
  [bunch of libraries of its own][294]. [``MIT``][MIT]
* [libdjb][295] - Collection of libraries doing various things. (Apparently)
  public domain.
* [mmx][296] - Collection of single-header libraries. Various licenses, all
  open source.
* [par][297] - Bunch of single-file libraries. [``MIT``][MIT]
* [Snippets][298] - Useful code snippets and header-only libraries.
  Public domain.
* [stb][299] - Range of single-file libraries. Public domain.
* [tinyheaders][300] - Collection of header-only libraries, primarily oriented
  toward game development. [``Zlib``][Zlib]
* [CCAN](http://ccodearchive.net/) - Modelled after Perl's CPAN, this is a big collection of C code that does stuff. The full list is [here](http://ccodearchive.net/list.html).
* [clib](https://github.com/clibs/clib) - Something of a package manager for C. Comes with a [bunch of libraries of its own](https://github.com/clibs/clib/wiki/Packages). [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [gnulib](https://www.gnu.org/software/gnulib/) - Collection of common GNU code.
* [libdjb](http://www.fefe.de/djb/) - Collection of libraries doing various things. [`(Apparently) Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [BurntSushi/clibs](https://github.com/BurntSushi/clibs) - A smattering of miscellaneous C libraries. Includes sane argument parsing, a thread-safe multi-producer/multi-consumer queue, and implementation of common data structures (hashmaps, vectors and linked lists).
* [RandyGaul/cute_headers](https://github.com/RandyGaul/cute_headers) - Collection of cross-platform one-file C/C++ libraries with no dependencies, primarily used for games
* [attractivechaos/klib](https://github.com/attractivechaos/klib) - A standalone and lightweight C library
* [breckinloggins/libuseful](https://github.com/breckinloggins/libuseful) - A collection of useful data structures, algorithms, and utilities for C programming
* [chadjoan/C-Survival-Kit](https://github.com/chadjoan/C-Survival-Kit) - A set of useful functions, data structures, and macros aimed at allowing more expressive and reliable C code.  Portability targets are OpenVMS and Linux.
* [clibs/clib](https://github.com/clibs/clib) - C package manager-ish
* [erimatnor/libckit](https://github.com/erimatnor/libckit) - A kit of C-based utilities and data structures.
* [floooh/sokol](https://github.com/floooh/sokol) - minimal cross-platform standalone C headers
* [gingerBill/gb](https://github.com/gingerBill/gb) - gb single-file public domain libraries for C & C++
* [gozfree/libraries](https://github.com/gozfree/libraries) - Basic libraries all written in c by gozfree, including network, event, config, log, hash, ipc, rpc, mem,  and so on
* [mackron/dr_libs](https://github.com/mackron/dr_libs) - A collection of public domain single-file libraries for C/C++.
* [mattiasgustavsson/libs](https://github.com/mattiasgustavsson/libs) - Single-file public domain libraries for C/C++
* [matteobertozzi/carthage](https://github.com/matteobertozzi/carthage) - Pure C Data Structure and Utils
* [napsy/libhelper](https://github.com/napsy/libhelper) - General functions and data structures for C
* [niklasfrykholm/nflibs](https://github.com/niklasfrykholm/nflibs) - A collection of interoperable minimalistic C libraries
* [nothings/stb](https://github.com/nothings/stb) - stb single-file public domain libraries for C/C++

## Special Purpose ##
* [Tulip Indicators][394] - Library of functions for technical analysis of
  financial data. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [libtrading][395] - Implementation of network protocols for communicating
  with exchanges, dark pools and other trading venues. Supports FIX, FIX/FAST
  and many proprietary protocols. [``BSD-2-Clause``][BSD-2-Clause]
* [AaronJackson/sage-in-c](https://github.com/AaronJackson/sage-in-c) - Simple library written in C for accessing invoices and company data created by Sage Accounts 50.
* [GuillaumeHolley/BloomFilterTrie](https://github.com/GuillaumeHolley/BloomFilterTrie) - A data structure for pan-genome storage
* [JayDDee/cpuminer-opt](https://github.com/JayDDee/cpuminer-opt) - Optimized multi algo CPU miner
* [MatthewLM/cbitcoin](https://github.com/MatthewLM/cbitcoin) - A low-level bitcoin library written in standard C.
* [Netflix/dynomite](https://github.com/Netflix/dynomite) - A generic dynamo implementation for different k-v storage engines
* [RhysU/ESIO](https://github.com/RhysU/ESIO) - The ExaScale IO (ESIO) library provides simple, high throughput input and output of structured data sets using parallel HDF5. ESIO is designed to support reading and writing turbulence simulation restart files within C, C++, and modern Fortran applications.
* [TPSully/SRTM2STL](https://github.com/TPSully/SRTM2STL) - Create STL files from SRTM data for the purpose of creating 3D relief maps.
* [TravisWhitaker/FermiShell](https://github.com/TravisWhitaker/FermiShell) - Retrieve, compare, calculate, analyze, graph, simulate, and experiment with chemical data.
* [TulipCharts/tulipindicators](https://github.com/TulipCharts/tulipindicators) - Technical Analysis Indicator Function Library in C
* [Unidata/netcdf-c](https://github.com/Unidata/netcdf-c) - Official GitHub repository for netCDF-C libraries and utilities.
* [XenonofArcticus/DynamicTrack](https://github.com/XenonofArcticus/DynamicTrack) - Access sources of dynamically-updated data about discrete entities like GPSes, INSes, ADS-B sources.
* [anza/metar](https://github.com/anza/metar) - METAR data fetcher and parser
* [bauerca/gridfloat](https://github.com/bauerca/gridfloat) - Slice and dice USGS elevation data from the command line.
* [cbuchner1/CudaMiner](https://github.com/cbuchner1/CudaMiner) - a CUDA accelerated litecoin mining application based on pooler's CPU miner
* [ericmandel/funtools](https://github.com/ericmandel/funtools) - A "minimal buy-in" FITS library and utility package for astronomical data analysis
* [geocommons/geocoder](https://github.com/geocommons/geocoder) - Modular Street Address Geocoder
* [jgarzik/cpuminer](https://github.com/jgarzik/cpuminer) - CPU miner for bitcoin
* [jgarzik/picocoin](https://github.com/jgarzik/picocoin) - A bitcoin library in C, SPV wallet & more.
* [libtrading/libtrading](https://github.com/libtrading/libtrading) - Libtrading, an ultra low-latency trading connectivity library for C and C++.
* [nayuki/QR-Code-generator](https://github.com/nayuki/QR-Code-generator) - High-quality QR Code generator library in Java, JavaScript, Python, C++, C.
* [noporpoise/seq_file](https://github.com/noporpoise/seq_file) - Library for Reading Bioinformatic Sequence Data in C

## Geography ##
Geodata, street maps, navigation and so on

* [libpostal][396] - Library for parsing and normalization of street addresses
  around the world. Powered by statistical NLP and open geo data. [``MIT``][MIT]
* [libgeohash][417] - Pure C implementation of the Geohash algorithm. [``BSD-3-Clause``][BSD-3-Clause]
* [Jahor/osm-tools](https://github.com/Jahor/osm-tools) - Tools to operate OpenStreetMap data
* [Unidata/gempak](https://github.com/Unidata/gempak) - Analysis, display, and product generation package for meteorological data.
* [aaronstanton/sualft](https://github.com/aaronstanton/sualft) - reconstruction of irregularly sampled seismic data using the Anti-Leakage Fourier Transform (ALFT)
* [evanmiller/ProjCL](https://github.com/evanmiller/ProjCL) - Crazy-fast map projections and geodesic calculations
* [olofsj/GLMap](https://github.com/olofsj/GLMap) - An OpenGL ES 2.0 renderer for Openstreetmap data
* [olofsj/Whichway](https://github.com/olofsj/Whichway) - C library for flexible (bike, foot, car) routing in road networks from Openstreetmap data.
* [maxmind/geoip-api-c](https://github.com/maxmind/geoip-api-c) - GeoIP Legacy C API
* [navit-gps/navit](https://github.com/navit-gps/navit) - The open source (GPL v2) turn-by-turn navigation software for many OS
* [lionsoul2014/ip2region](https://github.com/lionsoul2014/ip2region) - Ip2region is a offline IP location library with accuracy rate of 99.9% and 0.0x millseconds searching performance. DB file is less then 5Mb with all ip address stored. binding for Java,PHP,C,Python,Nodejs,Golang,C#,lua. Binary,B-tree,Memory searching algorithm
* [openvenues/libpostal](https://github.com/openvenues/libpostal) - A C library for parsing/normalizing street addresses around the world. Powered by statistical NLP and open geo data.

## Standard Libraries ##
Implementations of the C standarts

* [Bionic][301] - Google's standard library, developed for Android. [``BSD-3-Clause``][BSD-3-Clause]
* [cloudlibc][302] - Standard library based on the concept of
  [capability-based security][303]. [``BSD-2-Clause``][BSD-2-Clause]
* [dietlibc][304] - Standard library designed for the smallest possible
  binaries. [``GPL-2.0-only``][GPL-2.0-only]
* [glibc][305] - The GNU C Library; an implementation of the standard library. [``LGPL-2.1-only``][LGPL-2.1-only].
* [musl][306] - Standard library, compatible with POSIX 2008 and C11. Designed
  for static linking. [``MIT``][MIT]
* [PDCLib][307] - The Public Domain C Library. Implements most of C99 and some
  of C11. [``CC0-1.0``][CC0-1.0]
* [uClibc-ng][308] - Small C library for developing embedded systems.
  [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [Bionic](https://github.com/aosp-mirror/platform_bionic) - Google's C standard library, developed for Android. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [dietlibc](http://www.fefe.de/dietlibc/) - C standard library designed for the smallest possible binaries. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [glibc](http://www.gnu.org/software/libc/) - The GNU C Library; an implementation of the C standard library. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [musl](http://www.musl-libc.org/) - Standard C library, compatible with POSIX 2008 and C11. Designed for static linking. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [NuxiNL/cloudlibc](https://github.com/NuxiNL/cloudlibc) - CloudABI's standard C library
* [marssaxman/startc](https://github.com/marssaxman/startc) - minimal freestanding C library for bare-metal i386 development
* [olibc/olibc](https://github.com/olibc/olibc) - Another C Library optimized for Embedded Linux

## String Manipulation ##
* [bstring][309] - The Better String Library. [``BSD-3-Clause``][BSD-3-Clause]
* [ICU][310] - International Components for Unicode; a library for Unicode
  support. [``ICU``][ICU]
* [levenstein.c][311] - [Levenstein distance][312] algorithm implementation. [``MIT``][MIT].
* [libunistring][313] - Library for manipulating Unicode strings. [``LGPL-3.0-only``][LGPL-3.0-only]
* [libgiconv][314] - Text conversion library. [``LGPL-2.1-only``][LGPL-2.1-only]
* [librope][315] - UTF-8 rope ('heavy' string) library. [``MIT``][MIT]
* [rapidstring][316] - Maybe the fastest string library ever. [``MIT``][MIT]
* [SDS][317] - Simple Dynamic Strings; a library for handling strings in a
  simpler way, but one that is compatible with normal C string functions. [``BSD-2-Clause``][BSD-2-Clause]
* [stmr.c][318] - [Porter Stemmer][319] algorithm implementation. [``MIT``][MIT]
* [utf8.h][320] - Single-header UTF-8 library, designed to mimic C-style string
  functions. Public domain.
* [utf8proc][321] - Library for processing UTF-8 data. [``MIT``][MIT]
* [bstrlib](http://bstring.sourceforge.net/) - The Better String Library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause) and [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [ICU](http://site.icu-project.org/) - International Components for Unicode; a library for Unicode support. [`ICU license`](http://source.icu-project.org/repos/icu/icu/tags/latest/LICENSE)
* [libunistring](https://www.gnu.org/software/libunistring/) - Library for manipulating Unicode strings in C. [`GNU LGPL3`](http://www.gnu.org/licenses/lgpl.html)
* [libgiconv](https://www.gnu.org/software/libiconv/) - Text conversion library. [`GNU LGPL2.1 (library)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`GNU GPL3 (*iconv* program)`](http://www.gnu.org/licenses/gpl.html)
* [SDS](https://github.com/antirez/sds) - Simple Dynamic Strings; a library for handling C strings in a simpler way, but one that is compatible with normal C string functions. Available via [clib](https://github.com/clibs/clib). [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [shoco](http://ed-von-schleck.github.io/shoco/) - Compressor for small text strings. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [utf8.h](https://github.com/sheredom/utf8.h) - Single header utf8 string functions. [`Unlicense`](http://unlicense.org/)
* [utf8proc](https://github.com/JuliaStrings/utf8proc) - Small, clean library for processing UTF-8 Unicode data. [`License`](https://github.com/JuliaStrings/utf8proc/blob/master/LICENSE.md)
* [JuliaStrings/utf8proc](https://github.com/JuliaStrings/utf8proc) - a clean C library for processing UTF-8 Unicode data
* [antirez/sds](https://github.com/antirez/sds) - Simple Dynamic Strings library for C
* [boyerjohn/rapidstring](https://github.com/boyerjohn/rapidstring) - Maybe the fastest string library ever.
* [clibs/buffer](https://github.com/clibs/buffer) - Tiny C string library
* [cloudwu/cstring](https://github.com/cloudwu/cstring) - A simple C string lib
* [chrisjmccormick/word2vec_commented](https://github.com/chrisjmccormick/word2vec_commented) - Commented (but unaltered) version of original word2vec C implementation.
* [flori/amatch](https://github.com/flori/amatch) - Approximate String Matching library
* [fontforge/libuninameslist](https://github.com/fontforge/libuninameslist) - A library with a large (sparse) array mapping each unicode code point to the annotation data for it provided in http://www.unicode.org/Public/UNIDATA/NamesList.txt
* [jasonmaclafferty/String](https://github.com/jasonmaclafferty/String) - A dynamic string data type implementation for C.
* [josephg/librope](https://github.com/josephg/librope) - UTF-8 rope library for C

## Working With Files ##
Libraries for working wit hspecific filetypes

### Binaries ###
* [bfd][436] - Library for manipulating binary object files. Part of GNU
  binutils. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libelf][337] - Simple library for parsing ELF files. [``MIT``][MIT]
* [abiggerhammer/hammer](https://github.com/abiggerhammer/hammer) - Parser combinators for binary formats, in C. Yes, in C. What? Don't look at me like that.
* [anjos/arithmetic_coding](https://github.com/anjos/arithmetic_coding) - Library to perform arithmetic coding and decoding of text or binary data
* [beave/barnyard2-extra](https://github.com/beave/barnyard2-extra) - Barnyard2 with "Extra Data" support and other enhancements.
* [fuzxxl/memf](https://github.com/fuzxxl/memf) - Portable scanf/printf-like functions to marshal binary data
* [nicklockwood/FastCoding](https://github.com/nicklockwood/FastCoding) - A faster and more flexible binary file format replacement for NSCoding, Property Lists and JSON

### CSV ###
* [libcsv][322] - Simple, streaming CSV parser. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]

### JSON ###
* [Jansson][323] - Library for encoding, decoding and manipulating JSON. [``MIT``][MIT]
* [jfes][324] - JSON For Embedded Systems; simple JSON engine without any
  dependencies. [``MIT``][MIT]
* [jsmn][325] - Minimalistic JSON parser. [``MIT``][MIT]
* [json.h][326] - Single-file non-streaming JSON parser. [``Unlicense``][Unlicense]
* [WJElement][327] - Advanced JSON manipulation library, with support for JSON
  Schema. Various licenses, all open source.
* [YAJL][328] - Fast streaming JSON parser library. [``ISC``][ISC]
* [Jansson](http://www.digip.org/jansson/) - C library for encoding, decoding and manipulating JSON. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [jsmn](https://zserge.com/jsmn.html) - Minimalistic JSON parser. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [json-c](https://github.com/json-c/json-c/wiki) - Library for working with JSON. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [parson](https://github.com/kgabis/parson) - Lightweight JSON library written in C. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [WJElement](https://github.com/netmail-open/wjelement/wiki) - Advanced JSON manipulation library, with support for JSON Schema. [`LGPL, any version`](https://github.com/netmail-open/wjelement/)
* [YAJL](https://lloyd.github.io/yajl/) - Fast C JSON streaming parser library. [`ISC`](https://directory.fsf.org/wiki/License:ISC)
* [DaveGamble/cJSON](https://github.com/DaveGamble/cJSON) - Ultralightweight JSON parser in ANSI C
* [akheron/jansson](https://github.com/akheron/jansson) - C library for encoding, decoding and manipulating JSON data
* [armink/struct2json](https://github.com/armink/struct2json) - A fast convert library between the JSON and C structure. Implement structure serialization and deserialization for C. | C 结构体与 JSON 快速互转库，快速实现 C 结构体的序列化及反序列化
* [cesanta/frozen](https://github.com/cesanta/frozen) - JSON parser and generator for C/C++ with scanf/printf like interface. Targeting embedded systems.
* [cloudflare/lua-resty-json](https://github.com/cloudflare/lua-resty-json) - json lib for lua and C
* [esnme/ultrajson](https://github.com/esnme/ultrajson) - Ultra fast JSON decoder and encoder written in C with Python bindings
* [json-c/json-c](https://github.com/json-c/json-c) - https://github.com/json-c/json-c is the official code repository for json-c.  See the wiki for release tarballs for download.  API docs at http://json-c.github.io/json-c/
* [kbranigan/cJSON](https://github.com/kbranigan/cJSON) - I did not write this code, but I like it.
* [keenerd/jshon](https://github.com/keenerd/jshon) - Jshon is a JSON parser designed for maximum convenience within the shell.
* [kgabis/parson](https://github.com/kgabis/parson) - Lightweight JSON library written in C.
* [kevinbirch/kanabo](https://github.com/kevinbirch/kanabo) - query JSON/YAML data with JSONPath
* [lloyd/yajl](https://github.com/lloyd/yajl) - A fast streaming JSON parsing library in C.
* [mysqludf/lib_mysqludf_json](https://github.com/mysqludf/lib_mysqludf_json) - A UDF library of functions to map relational data to the JSON format.
* [netmail-open/wjelement](https://github.com/netmail-open/wjelement) - advanced, flexible JSON manipulation in C
* [orangeduck/json2c](https://github.com/orangeduck/json2c) - Convert JSON to C data literals

### INI ###
* [inih][329] - Small and simple INI file parser, good for embedded systems. [``BSD-3-Clause``][BSD-3-Clause]
* [iniparser][330] - Parser for .ini files. [``MIT``][MIT]
* [libconfini][331] - Yet another INI parser. [``GPL-3.0-only``][GPL-3.0-only]
* [benhoyt/inih](https://github.com/benhoyt/inih) - Simple .INI file parser in C, good for embedded systems

### Markdown ###
* [Hoedown][375] - Fully standards-compliant, extension-supporting, UTF-8
  aware, fast Markdown parser. [``MIT``][MIT]
* [libcmark][376] - Library for parsing the CommonMark dialect of
  Markdown. [``BSD-2-Clause``][BSD-2-Clause]
* [Discount][377] - Simple implementation of a Markdown parser. [``BSD-3-Clause``][BSD-3-Clause]
* [cmark][420] - Implementation of the CommonMark, Markdown dialect.
  [Variety of licenses, all open source][421].
* [Orc/discount](https://github.com/Orc/discount) - My C implementation of John Gruber's Markdown markup language
* [ali-rantakari/peg-markdown-highlight](https://github.com/ali-rantakari/peg-markdown-highlight) - C library for Markdown syntax highlighting, using a recursive-descent parser.
* [commonmark/cmark](https://github.com/commonmark/cmark) - CommonMark parsing and rendering library and program in C
* [commonsguy/cwac-anddown](https://github.com/commonsguy/cwac-anddown) - CWAC AndDown: Markdown Utility Library
* [fletcher/MultiMarkdown-4](https://github.com/fletcher/MultiMarkdown-4) - C implementation of MultiMarkdown; almost complete rewrite of MMD 3 (which was aka "peg-multimarkdown").
* [jgm/cmark](https://github.com/jgm/cmark) - CommonMark parsing and rendering library and program in C
* [jgm/peg-markdown](https://github.com/jgm/peg-markdown) - An implementation of markdown in C, using a PEG grammar

### XML ###
* [Expat][332] - Stream-oriented XML parser. [MIT][MIT]
* [libxml2][333] - Standards-compliant, portable XML parser. [MIT][MIT]
* [mini-xml](https://github.com/michaelrsweet/mxml) - Small XML reading and writing library. No dependencies aside from C standard library. [`GNU LGPL2.1 with static linking exception`](https://github.com/michaelrsweet/mxml/blob/master/COPYING)
* [CastXML/CastXML](https://github.com/CastXML/CastXML) - C-family Abstract Syntax Tree XML Output
* [TouchCode/TouchXML](https://github.com/TouchCode/TouchXML) - Official "clone" of TouchXML from TouchCode
* [libexpat/libexpat](https://github.com/libexpat/libexpat) - :herb: Expat library: Fast streaming XML parser written in C; in the process of migrating from SourceForge to GitHub

### YAML ###
* [libYAML][334] - YAML 1.1 parser and emitter. [``MIT``][MIT]

### Other Filetypes ###
* [libbson][335] - BSON utility library. [``Apache-2.0``][Apache-2.0]
* [libconfuse][336] - Small configuration file parser library. [``ISC``][ISC]
* [libucl][338] - Universal configuration library parser. [``BSD-2-Clause``][BSD-2-Clause]
* [libxo][339] - Allows an application to generate plain text, XML, JSON and
  HTML output using a common set of function calls. The application decides at
  runtime what output style should be produced. [``BSD-2-Clause``][BSD-2-Clause]
* [XLSX I/O][413] - Cross-platform library for reading and writing .xlsx files. [``MIT``][MIT]
* [gumbo-parser][416] - HTML5 parsing library in C99. [``Apache-2.0``][Apache-2.0]
* [hammer](https://github.com/abiggerhammer/hammer) - Parser combinators for binary formats. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [iniparser](https://github.com/ndevilla/iniparser) - Parser for `.ini` files. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libconfini](https://github.com/madmurphy/libconfini) - Yet another INI parser. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [libYAML](https://pyyaml.org/wiki/LibYAML) - YAML 1.1 parser and emitter. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [mpc](https://github.com/orangeduck/mpc) - Parser combinator library. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [libucl](https://github.com/vstakhov/libucl) - Universal configuration library parser. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [StefanKarpinski/odb](https://github.com/StefanKarpinski/odb) - ODB: On-Disk Binary Data Tool
* [WizardMac/ReadStat](https://github.com/WizardMac/ReadStat) - Command-line tool (+ C library) for converting SAS, Stata, and SPSS files
* [arrbee/diff-match-patch-c](https://github.com/arrbee/diff-match-patch-c) - C language port of google-diff-match-patch library
* [clarkgrubb/data-tools](https://github.com/clarkgrubb/data-tools) - File format conversion tools
* [fileability/self-ml](https://github.com/fileability/self-ml) - A human data language
* [hach-que/configd](https://github.com/hach-que/configd) - Generates configuration files in /etc based on YAML data and XSLT transformations.
* [hyperrealm/libconfig](https://github.com/hyperrealm/libconfig) - C/C++ library for processing configuration files
* [jedwing/CHMLib](https://github.com/jedwing/CHMLib) - Library for reading Microsoft ITSS/CHM format files.
* [jmcnamara/libxlsxwriter](https://github.com/jmcnamara/libxlsxwriter) - A C library for creating Excel XLSX files.
* [jwerle/fs.c](https://github.com/jwerle/fs.c) - File system API much like Node's fs module
* [libharu/libharu](https://github.com/libharu/libharu) - libharu - free PDF library
* [martinh/libconfuse](https://github.com/martinh/libconfuse) - Small configuration file parser library for C.
* [mw55309/c_fast5](https://github.com/mw55309/c_fast5) - C code to extract data from fast5 files

--------------------------------------------------------------------------------

## Testing ##
* [CHEAT][340] - Simple unit testing framework. [``BSD-2-Clause``][BSD-2-Clause]
* [Check][341] - Unit testing framework. [``LGPL-2.1-only``][LGPL-2.1-only]
* [ciut][342] - A modern minimal hassle unit test framework. [``MIT``][MIT]
* [clar][343] - Clear and simple unit testing framework. [``MIT``][MIT]
* [CMock][344] - Mock/stub generator. [``MIT``][MIT]
* [cmocka][345] - Unit testing framework with support for mock objects. [``Apache-2.0``][Apache-2.0]
* [Criterion][346] - KISS, non-intrusive test framework. [``MIT``][MIT]
* [ctest][347] - Yet another unit testing framework. [``Apache-2.0``][Apache-2.0]
* [CUnit][348] - Another unit testing framework. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [greatest][349] - Unit testing library in one file, with no memory allocation. [``MIT``][MIT]
* [minctest][350] - Unit testing microlibrary. [``BSD-3-Clause``][BSD-3-Clause]
* [munit][351] - Small unit testing framework. [``MIT``][MIT]
* [theft][352] - Property-based testing (similar to [Quickcheck][353]). [``MIT``][MIT]
* [Unity][354] - Simple unit testing framework. [``MIT``][MIT]
* [utest][355] - Single-header unit testing library. [``Unlicense``][Unlicense]
* [CHEAT](http://users.jyu.fi/~sapekiis/cheat/) - Very simple unit testing framework. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [Check](https://libcheck.github.io/check/) - Unit testing framework for C. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [CMock](http://www.throwtheswitch.org/) - Mock/stub generator for C. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [cmocka](https://cmocka.org/) - Unit testing framework with support for mock objects. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [Criterion](https://criterion.readthedocs.io/en/master/) - KISS, non-intrusive C test framework. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [CUnit](http://cunit.sourceforge.net/) - Another unit testing framework for C. [`GNU LGPL2.0`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [Cutest](https://github.com/rafael-santiago/cutest) - Library for unit testing with memory leak detection (Linux, freeBSD and Windows). [`GPL2`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [minunit](https://github.com/siu/minunit) - Minimal unit testing framework for C. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [munit](https://nemequ.github.io/munit/) - Small but full-featured unit testing framework for C with no dependencies. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [Unity](http://www.throwtheswitch.org/) - Simple unit testing framework for C. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [zorgnax/libtap](https://github.com/zorgnax/libtap) - Write tests in C
* [Snaipe/Criterion](https://github.com/Snaipe/Criterion) - A cross-platform C and C++ unit testing framework for the 21th century
* [ThrowTheSwitch/Unity](https://github.com/ThrowTheSwitch/Unity) - Simple Unit Testing for C
* [bvdberg/ctest](https://github.com/bvdberg/ctest) - ctest is a unit test framework for software written in C.
* [clear-code/cutter](https://github.com/clear-code/cutter) - An easy to write and debug unit testing framework for C and C++.
* [compiler-dept/speck](https://github.com/compiler-dept/speck) - A small unit testing framework for C
* [joewalnes/tinytest](https://github.com/joewalnes/tinytest) - A tiny unit-testing framework for C
* [libcheck/check](https://github.com/libcheck/check) - A unit testing framework for C
* [lpabon/cmockery2](https://github.com/lpabon/cmockery2) - Reviving cmockery unit test framework from Google
* [mcandre/qc](https://github.com/mcandre/qc) - qc - A C port of the QuickCheck unit test framework
* [mchochlov/Gnucash](https://github.com/mchochlov/Gnucash) - Data model unit testing - GSoC 2011
* [mortie/snow](https://github.com/mortie/snow) - A testing library for C.
* [orangeduck/ptest](https://github.com/orangeduck/ptest) - DRY Microtesting Framework for C

## TUI ##
Textual User Interface
* [progressbar][371] - Easy-to-use library for displaying text progress bars. [``BSD-3-Clause``][BSD-3-Clause]
* [netbsd-curses][372] - Simplified and small version of ncurses, with the same
  interface. [``BSD-3-Clause``][BSD-3-Clause]
* [ncurses][373] - Coloured terminal UI library. [``MIT``][MIT]
* [termbox][374] - Library for writing text-based interfaces. [``MIT``][MIT]
* [bartobri/bmenu](https://github.com/bartobri/bmenu) - A generic terminal menu written in C.
* [doches/progressbar](https://github.com/doches/progressbar) - An easy-to-use C library for displaying text progress bars.
* [hpjansson/chafa](https://github.com/hpjansson/chafa) - 📺🗿 Terminal graphics for the 21st century.
* [jwerle/progress.c](https://github.com/jwerle/progress.c) - Progress display lib for c
* [nsf/termbox](https://github.com/nsf/termbox) - Library for writing text-based user interfaces

## Web Frameworks ##
Comprehensive and integrated solutions for building web application in C.
* [Cloudgizer][361] - Cloudgizer is a tool for building web applications as
  Apache modules, with emphasis on performance, small-footprint, and more
  productive and safer programming in C. [``Apache-2.0``][Apache-2.0]
* [facil.io][362] - Mini-framework for web applications. Includes a fast HTTP
  and Websocket server, and also supports custom protocols. [``MIT``][MIT]
* [KLone][363] - Fully featured, multi-platform, web application development
  framework, targeted especially at embedded systems and appliances. [``BSD-3-Clause``][BSD-3-Clause]
* [Kore][364] - Easy-to-use web application framework for writing scalable
  web APIs in C. [``ISC``][ISC]
* [WAFer][378] - Ultra-light software platform for scalable server-side and
  networking applications (think node.js for C programmers). [``GPL-2.0-only``][GPL-2.0-only]
* [balde](https://balde.rgm.io/) - Microframework for C based on GLib. [`GNU LGPLv2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [onion](https://www.coralbits.com/libonion/) - C library to create simple HTTP servers and Web Applications. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [kore](https://kore.io/) - Easy to use, scalable and secure web application framework for writing web APIs in C.
* [klone](http://www.koanlogic.com/klone/) - KLone is a fully-featured, multiplatform, web application development framework.
* [duda](http://duda.io/) - Duda I/O is an event-driven and high performant web services framework written in C. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [DanielWaterworth/Raphters](https://github.com/DanielWaterworth/Raphters) - [DEPRECATED] A web framework for C.
* [babelouest/ulfius](https://github.com/babelouest/ulfius) - Web Framework to build REST APIs, Webservices or any HTTP endpoint in C language. Can stream large amount of data, integrate JSON data with Jansson, and create websocket services
* [bitly/simplehttp](https://github.com/bitly/simplehttp) - a family of libraries and daemons for building scalable web infrastructure
* [boazsegev/facil.io](https://github.com/boazsegev/facil.io) - Your high performance web application C framework
* [ccxvii/mujs](https://github.com/ccxvii/mujs) - An embeddable Javascript interpreter in C.
* [cesanta/mongoose](https://github.com/cesanta/mongoose) - Embedded web server for C/C++
* [cesanta/smart.js](https://github.com/cesanta/smart.js) - Embedded Javascript engine for C/C++ with networking, file, database and device interfaces
* [cesanta/v7](https://github.com/cesanta/v7) - Embedded JavaScript engine for C/C++
* [criticalstack/libevhtp](https://github.com/criticalstack/libevhtp) - Create extremely-fast and secure embedded HTTP servers with ease.
* [danielwaterworth/Raphters](https://github.com/danielwaterworth/Raphters) - [DEPRECATED] A web framework for C.
* [davidmoreno/onion](https://github.com/davidmoreno/onion) - C library to create simple HTTP servers and Web Applications.
* [embedthis/appweb](https://github.com/embedthis/appweb) - Appweb Embedded Web Server
* [haiwen/ccnet](https://github.com/haiwen/ccnet) - Ccnet is a framework for writing networked applications in C.
* [haywire/haywire](https://github.com/haywire/haywire) - Haywire is an asynchronous HTTP server framework written in C that's built using the event loop based libuv platform layer that node.js is built on top of.
* [iafonov/cosmonaut](https://github.com/iafonov/cosmonaut) - Fast web server & micro framework implemented in C. Just for fun.
* [it4e/CHL](https://github.com/it4e/CHL) - C Hypertext Library - A library for writing web applications in C
* [jorisvink/kore](https://github.com/jorisvink/kore) - An easy to use, scalable and secure web application framework for writing web APIs in C. || This is a read-only mirror, please see https://kore.io/mail and https://kore.io/source for information on how to contribute via the mailing lists.
* [kellabyte/Haywire](https://github.com/kellabyte/Haywire) - Haywire is an asynchronous HTTP server framework written in C that's built using the event loop based libuv platform layer that node.js is built on top of.
* [monkey/duda](https://github.com/monkey/duda) - Duda I/O is an event-driven and high performant web services framework which exposes a friendly C API
* [oneoo/alilua](https://github.com/oneoo/alilua) - epoll/kqueue+lua based web server

## Web Service APIs ##
* [twitc][426] - Mini library for interacting with the Twitter OAuth API. [``MIT``][MIT]
* [dajobe/flickcurl](https://github.com/dajobe/flickcurl) - Flickr C API library
* [Cotix/cReddit](https://github.com/Cotix/cReddit) - CLI Reddit client written in C. Oh, crossplatform too!
* [HalosGhost/shaman](https://github.com/HalosGhost/shaman) - A small, native C library and utility to fetch weather
* [PromyLOPh/pianobar](https://github.com/PromyLOPh/pianobar) - Console-based pandora.com player
* [TOTBWF/SteamCurses](https://github.com/TOTBWF/SteamCurses) - A Basic NCurses Client for Steam
* [Yubico/yubico-c-client](https://github.com/Yubico/yubico-c-client) - Yubico C client library
* [adobkin/libcapn](https://github.com/adobkin/libcapn) - A simple C Library for interact with the Apple Push Notification Service (APNs)
* [andrewstone/AbqData](https://github.com/andrewstone/AbqData) - Tools to read ABQ Open Data Initiative city gov data
* [aws/aws-iot-device-sdk-embedded-C](https://github.com/aws/aws-iot-device-sdk-embedded-C) - SDK for connecting to AWS IoT from a device using embedded C.

[424]: http://coap.technology/

# Uncategorized #
* [tm][432] -  Timer and Timeline Utils for C. [``MIT``][MIT]
* [D-Bus][430] - Interprocess communications bus. [``AFL-2.1``][AFL-2.1] or [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [libgit2](https://libgit2.org/) - Pure C implementation of Git. [`GNU GPL2 only, with a linking exception`](https://github.com/libgit2/libgit2/blob/master/COPYING)
* [Keruspe/GPaste](https://github.com/Keruspe/GPaste) - Clipboard management system
* [Lajnold/falloc](https://github.com/Lajnold/falloc) - falloc creates files of a user-specified size. It uses the posix_fallocate syscall for allocating the right size directly, instead of copying data like the commonly used dd tool does (which, in my opinion, feels like a hack).
* [ThomasHabets/monotonic_clock](https://github.com/ThomasHabets/monotonic_clock) - Portable C library for getting monotonic time
* [WhisperSystems/libsignal-protocol-c](https://github.com/WhisperSystems/libsignal-protocol-c) - Signal Protocol C Library
* [alandekok/recli](https://github.com/alandekok/recli) - A re-imagined CLI.  Customizable syntax, help, permissions, data types.
* [armon/statsite](https://github.com/armon/statsite) - C implementation of statsd
* [bus1/dbus-broker](https://github.com/bus1/dbus-broker) - Linux D-Bus Message Broker
* [cesanta/mjs](https://github.com/cesanta/mjs) - Embedded JavaScript engine for C/C++
* [cgaebel/pipe](https://github.com/cgaebel/pipe) - A simple thread-safe FIFO in C.
* [cloudyourcar/minmea](https://github.com/cloudyourcar/minmea) - a lightweight GPS NMEA 0183 parser library in pure C
* [couchbase/libcouchbase](https://github.com/couchbase/libcouchbase) - The couchbase client for C.
* [cxong/tinydir](https://github.com/cxong/tinydir) - Lightweight, portable and easy to integrate C directory and file reader
* [dmw/caffeine](https://github.com/dmw/caffeine) - C Application Framework
* [douban/greenify](https://github.com/douban/greenify) - Make blocking C library work with gevent
* [droe/sslsplit](https://github.com/droe/sslsplit) - Transparent SSL/TLS interception
* [drvink/epanos](https://github.com/drvink/epanos) - ElectroPaint Automatic No-source Object reaSsembler (a MIPS to C decompiler)
* [eam/libcrange](https://github.com/eam/libcrange) - Range parsing library for managing sets of hostnames, ips, clusters, roles and other operational data.
* [editorconfig/editorconfig-core-c](https://github.com/editorconfig/editorconfig-core-c) - EditorConfig core library written in C (for use by plugins supporting EditorConfig parsing)
* [ellson/graphviz](https://github.com/ellson/graphviz) - Graph Visualization Tools
* [elvismt/slope](https://github.com/elvismt/slope) - A library to create charts from raw data using cairo. Can be shown in GtkDrawingArea
* [fomy/destor](https://github.com/fomy/destor) - An experimental platform for chunk-level data deduplication. Key words: DDFS, Sparse Index, Extreme Binning, SiLo, Sample Index, BLC; CBR, CFL, CAP, HAR; ASM, OPT; GC, Cumulus
* [freefoote/gpscorrelate](https://github.com/freefoote/gpscorrelate) - Abandoned C program to match GPS tracks to photographs, and store the matches in the EXIF data in the photographs.
* [graphitemaster/incbin](https://github.com/graphitemaster/incbin) - Include binary files in C/C++
* [h2non/semver.c](https://github.com/h2non/semver.c) - semantic version parser and serializer written in ANSI C
* [hmng/jsonrpc-c](https://github.com/hmng/jsonrpc-c) - JSON-RPC in C (server only for now)
* [hroptatyr/dateutils](https://github.com/hroptatyr/dateutils) - nifty command line date and time utilities; fast date calculations and conversion in the shell
* [hroptatyr/uterus](https://github.com/hroptatyr/uterus) - universal tick encoder library to efficiently transport huge amounts of tick data
* [htacg/tidy-html5](https://github.com/htacg/tidy-html5) - The granddaddy of HTML tools, with support for modern standards
* [jkff/scrunch](https://github.com/jkff/scrunch) - Stream cruncher - data stream algorithms
* [jonpe960/ufsm](https://github.com/jonpe960/ufsm) - UML Statechart library in C and XMI importer
* [juliettef/IconFontCppHeaders](https://github.com/juliettef/IconFontCppHeaders) - C, C++ headers and C# classes for icon fonts: Font Awesome, Fork Awesome, Material Design, Material Design icons, Kenney game icons and Ionicons
* [kosma/minmea](https://github.com/kosma/minmea) - a lightweight GPS NMEA 0183 parser library in pure C
* [lexborisov/Modest](https://github.com/lexborisov/Modest) - Modest is a fast HTML renderer implemented as a pure C99 library with no outside dependencies.
* [lexborisov/myhtml](https://github.com/lexborisov/myhtml) - Fast C/C++ HTML 5 Parser. Using threads.
* [libgit2/libgit2](https://github.com/libgit2/libgit2) - The Library
* [libical/libical](https://github.com/libical/libical) - Libical is an Open Source implementation of the iCalendar protocols and protocol data units.
* [lopter/lightsd](https://github.com/lopter/lightsd) - A daemon with a JSON-RPC API to control your light bulbs
* [locasto/libdisorder](https://github.com/locasto/libdisorder) - A simple C library for entropy measurement of byte streams and other data.
* [lucasb-eyer/heatmap](https://github.com/lucasb-eyer/heatmap) - High performance C heatmap generation library. Supposed to be wrapped by higher-level languages.
* [luke-jr/bfgminer](https://github.com/luke-jr/bfgminer) - Modular ASIC/FPGA miner written in C, featuring overclocking, monitoring, fan speed control and remote interface capabilities.
* [luohaha/CSpider](https://github.com/luohaha/CSpider) - A scalable and convenient crawler framework in C:).
* [mhroth/tinyosc](https://github.com/mhroth/tinyosc) - A minimal Open Sound Control (OSC) library written in vanilla C.
* [mongrel2/mongrel2](https://github.com/mongrel2/mongrel2) - The Mongrel2 Web Server Project
* [nikhilm/uvbook](https://github.com/nikhilm/uvbook) - An Introduction to libuv
* [nitrogenlogic/cliserver](https://github.com/nitrogenlogic/cliserver) - A sample libevent-based network socket server that presents a simple command line interface to multiple connecting clients.
* [nlsandler/write_a_c_compiler](https://github.com/nlsandler/write_a_c_compiler) - Test suite to help you write your own C compiler
* [openglbook/openglbook.com](https://github.com/openglbook/openglbook.com) - The source code for http://openglbook.com/
* [openglsuperbible/sb6code](https://github.com/openglsuperbible/sb6code) - Source code for OpenGL SupeBible 6th Edition examples
* [openglsuperbible/sb7code](https://github.com/openglsuperbible/sb7code) - Source code and supporting material for the 7th Edition of OpenGL SuperBible
* [orlp/ed25519](https://github.com/orlp/ed25519) - Portable C implementation of Ed25519, a high-speed high-security public-key signature system.
* [parallella/pal](https://github.com/parallella/pal) - An optimized C library for math, parallel processing and data movement

# Unsorted #
* [php/php-src](https://github.com/php/php-src) - The PHP Interpreter
* [pi-hole/FTL](https://github.com/pi-hole/FTL) - The Pi-hole FTL engine
* [pi8027/libdatastruct](https://github.com/pi8027/libdatastruct) - libdatastruct is an ANSI C library for abstract data types.
* [pikelang/Pike](https://github.com/pikelang/Pike) - Pike is a dynamic programming language with a syntax similar to Java and C. It is simple to learn, does not require long compilation passes and has powerful built-in data types allowing simple and really fast data manipulation.
* [pimoroni/unicorn-hat](https://github.com/pimoroni/unicorn-hat) - C library, C example and Python wrapper for driving ws2812 pixels from the Raspberry Pi
* [pipelinedb/pipelinedb](https://github.com/pipelinedb/pipelinedb) - The Streaming SQL Database
* [pixelnerve/BlockOpenNI](https://github.com/pixelnerve/BlockOpenNI) - A c++ wrapper for OpenNI.
* [pjotrp/biolib](https://github.com/pjotrp/biolib) - BioLib brings together a set of opensource libraries written in C/C++ and makes them available for all Bio* languages
* [pkieltyka/stash](https://github.com/pkieltyka/stash) - Steganography application that hides data within a bitmap image
* [pkmital/StickFigureOSC](https://github.com/pkmital/StickFigureOSC) - Streams PrimeSense NITE's Skeleton Data via OSC (XCode Project)
* [pkmital/pkmColorBlobTracker](https://github.com/pkmital/pkmColorBlobTracker) - track overhead using color and map tracked points to a new geometry using a homography transformation and calibration routine - some example test videos are provided in the bin/data directory of an overhead capture.  The tracking transformation is useful for when you need a defined metric space of your tracking parameters, or need to account for different user heights in tracking their paths in a space.
* [pkrumins/bithacks.h](https://github.com/pkrumins/bithacks.h) - bithacks.h is a C header file containing useful bit manipulation macros
* [pkrumins/node-base64](https://github.com/pkrumins/node-base64) - A base64 encoding and decoding C++ module for node.js that actually works! (node now has it's own base64 encoding, see docs!)
* [pkrumins/node-png](https://github.com/pkrumins/node-png) - A nodejs C++ module that given a buffer with RGB or RGBA values creates a PNG image (in memory).
* [planetbeing/iphonelinux](https://github.com/planetbeing/iphonelinux) - Port Linux to the iPhone
* [planetbeing/xpwn](https://github.com/planetbeing/xpwn) - A cross-platform custom NOR firmware loader and custom IPSW generator for the iPhone
* [plashchynski/str2hex](https://github.com/plashchynski/str2hex) - Data formats convertion utility
* [plusvic/yara](https://github.com/plusvic/yara) - The pattern matching swiss knife
* [pmq20/ruby-compiler](https://github.com/pmq20/ruby-compiler) - Ahead-of-time (AOT) Compiler designed for Ruby, that just works.
* [pmwkaa/sophia](https://github.com/pmwkaa/sophia) - modern emeddable key-value database
* [pn2200/g3data](https://github.com/pn2200/g3data) - Grab graph data, a program for extracting data from graphs
* [pocoproject/poco](https://github.com/pocoproject/poco) - The POCO C++ Libraries are powerful cross-platform C++ libraries for building network- and internet-based applications that run on desktop, server, mobile, IoT, and embedded systems.
* [pod2g/sendrawpdu](https://github.com/pod2g/sendrawpdu) - CLI tool to send raw SMS PDU data to the iPhone 4 baseband
* [popoffka/i3lock](https://github.com/popoffka/i3lock) - i3lock is a simple screen locker like slock. This repo contains a patched version of i3lock which displays additional data on the lock screen, such as current time (like this: http://nn.lv/3y1s).
* [pornel/dssim](https://github.com/pornel/dssim) - Image similarity comparison simulating human perception (multiscale SSIM in C)
* [pornel/giflossy](https://github.com/pornel/giflossy) - Lossy GIF compressor
* [pornel/pngquant](https://github.com/pornel/pngquant) - Lossy PNG compressor — pngquant command and libimagequant library
* [pornin/CTTK](https://github.com/pornin/CTTK) - Constant-Time Toolkit
* [postgis/postgis](https://github.com/postgis/postgis) - PostGIS spatial database extension to PostgreSQL
* [postgres/postgres](https://github.com/postgres/postgres) - Mirror of the official PostgreSQL GIT repository. Note that this is just a *mirror* - we don't work with pull requests on github. To contribute, please see http://wiki.postgresql.org/wiki/Submitting_a_Patch
* [posva/catimg](https://github.com/posva/catimg) - :squirrel: Insanely fast image printing in your terminal
* [powturbo/TurboRLE](https://github.com/powturbo/TurboRLE) - Fastest Run Length Encoding
* [pozorvlak/libtap](https://github.com/pozorvlak/libtap) - Testing library for C, implementing the Test Anything Protocol. Written by Nik Clayton.
* [pramsey/pgsql-ogr-fdw](https://github.com/pramsey/pgsql-ogr-fdw) - PostgreSQL foreign data wrapper for OGR
* [preshing/CompareIntegerMaps](https://github.com/preshing/CompareIntegerMaps) - Generates benchmark data for two different data structures, then renders some graphs.
* [prideout/par](https://github.com/prideout/par) - single-file C libraries from Philip Allan Rideout
* [priitj/whitedb](https://github.com/priitj/whitedb) - WhiteDB memory database
* [pritambaral/hostapd-rtl871xdrv](https://github.com/pritambaral/hostapd-rtl871xdrv) - Hostapd driver for RTL8188{C|CU|CUS} wifi chips.
* [probablycorey/seriously](https://github.com/probablycorey/seriously) - The Objective-C HTTP library that Apple should have created, seriously.
* [probablycorey/wax](https://github.com/probablycorey/wax) - Wax is now being maintained by alibaba
* [processhacker/processhacker](https://github.com/processhacker/processhacker) - A free, powerful, multi-purpose tool that helps you monitor system resources, debug software and detect malware.
* [processhacker2/processhacker2](https://github.com/processhacker2/processhacker2) - A free, powerful, multi-purpose tool that helps you monitor system resources, debug software and detect malware.
* [processhacker2/processhacker](https://github.com/processhacker2/processhacker) - A free, powerful, multi-purpose tool that helps you monitor system resources, debug software and detect malware.
* [processone/oneteam](https://github.com/processone/oneteam) - OneTeam XMPP multi-platform client. This is a Mozilla / XUL based platform, developed mostly in Javascript and C++ XPCOM.
* [proftpd/proftpd](https://github.com/proftpd/proftpd) - ProFTPD source code
* [programmingthomas/ObjectiveGumbo](https://github.com/programmingthomas/ObjectiveGumbo) - An Objective-C wrapper with utility functions around Gumbo for easy HTML5 parsing in Cocoa and Cocoa Touch
* [project-imas/security-check](https://github.com/project-imas/security-check) - Application level, attached debug detect and jailbreak checking
* [projectNe10/Ne10](https://github.com/projectNe10/Ne10) - An open optimized software library project for the ARM® Architecture
* [proot-me/PRoot](https://github.com/proot-me/PRoot) - chroot, mount --bind, and binfmt_misc without privilege/setup for Linux
* [propublica/simple-tiles](https://github.com/propublica/simple-tiles) - Simple tile generation for maps.
* [psankar/simplefs](https://github.com/psankar/simplefs) - A simple, kernel-space, on-disk filesystem from the scratch
* [pseudomuto/c-data-structures](https://github.com/pseudomuto/c-data-structures) - A simple library of data structures for C
* [psgroove/psgroove](https://github.com/psgroove/psgroove) - PSGroove
* [psobot/ipsumcrypt](https://github.com/psobot/ipsumcrypt) - A small C program to embed binary data into the whitespace between words.
* [psychs/cocoaoniguruma](https://github.com/psychs/cocoaoniguruma) - Objective-C binding of Oniguruma regular expression engine
* [pudongqi/My_Compiler](https://github.com/pudongqi/My_Compiler) - An open-source projects about how to develop a compiler
* [puffnfresh/toggle-osx-shadows](https://github.com/puffnfresh/toggle-osx-shadows) - Tiny tool to toggle window shadows on OS X
* [pure-data/pure-data](https://github.com/pure-data/pure-data) - Pure Data - tracking Miller's SourceForge git repository (also used by libpd)
* [pusher/libPusher](https://github.com/pusher/libPusher) - An Objective-C interface to Pusher | owner=@TomKemp
* [pvaret/rtl8192cu-fixes](https://github.com/pvaret/rtl8192cu-fixes) - Realtek 8192 chipset driver, ported to kernel 3.11.
* [pyca/pynacl](https://github.com/pyca/pynacl) - Python binding to the Networking and Cryptography (NaCl) library
* [pygame/pygame](https://github.com/pygame/pygame) - pygame (the library) is a Free and Open Source python programming language library for making multimedia applications like games built on top of the excellent SDL library. C, Python, Native, OpenGL.
* [pyknite/catwm](https://github.com/pyknite/catwm) - catwm is a very simple tiling window manager
* [pysam-developers/pysam](https://github.com/pysam-developers/pysam) - Pysam is a Python module for reading and manipulating SAM/BAM/VCF/BCF files. It's a lightweight wrapper of the htslib C-API, the same one that powers samtools, bcftools, and tabix.
* [python-greenlet/greenlet](https://github.com/python-greenlet/greenlet) - Lightweight in-process concurrent programming
* [q3k/gm_datapack](https://github.com/q3k/gm_datapack) - A binary Lua module for Garry's Mod to tell when a datapack is created.
* [qayshp/TestDisk](https://github.com/qayshp/TestDisk) - TestDisk is powerful free data recovery software!
* [qemu/qemu](https://github.com/qemu/qemu) - Official QEMU mirror
* [qianshanhai/fastwiki](https://github.com/qianshanhai/fastwiki) - Fast offline data reader
* [qiq/Czech-morphology](https://github.com/qiq/Czech-morphology) - Czech morphology library, using data files compatible with PDT 2.0
* [qmk/qmk_firmware](https://github.com/qmk/qmk_firmware) - keyboard controller firmware for Atmel AVR and ARM USB families
* [qris/iptables](https://github.com/qris/iptables) - Modified iptables binary for firewall data gathering via JSON
* [quantcast/qfs](https://github.com/quantcast/qfs) - Quantcast File System
* [quartzjer/js0n](https://github.com/quartzjer/js0n) - Flexible Zero-Footprint JSON Parser in C
* [qubodup/freedink-data](https://github.com/qubodup/freedink-data) - freedink-data sound additions. see http://www.freedink.org/ (not my project)
* [questor/ringbuffer](https://github.com/questor/ringbuffer) - simple ringbuffer with possibility to get all data and/or only updates
* [r-medina/ll](https://github.com/r-medina/ll) - Thread safe linked list data structure for C
* [r03ert0/CoactivationMap.app](https://github.com/r03ert0/CoactivationMap.app) - Interactive viewer for the Brain Coactivation Map data
* [r0nk/corvus](https://github.com/r0nk/corvus) - Genetic BF programming
* [rabbitmq/rabbitmq-c](https://github.com/rabbitmq/rabbitmq-c) - The official rabbitmq-c sources have moved to:
* [rackerlabs/boot.rackspace.com](https://github.com/rackerlabs/boot.rackspace.com) - Multiple Operating System Installer via iPXE
* [radare/radare2](https://github.com/radare/radare2) - unix-like reverse engineering framework and commandline tools security
* [radareorg/r2con](https://github.com/radareorg/r2con) - Radare Congress Stuff
* [radarsat1/plhm](https://github.com/radarsat1/plhm) - A library and command-line front-end for acquiring data from Polhemus motion tracking devices.
* [radfordneal/LDPC-codes](https://github.com/radfordneal/LDPC-codes) - Software for Low Density Parity Check codes
* [radif/SIPHON-SIP-Client-that-actually-compiles](https://github.com/radif/SIPHON-SIP-Client-that-actually-compiles) - SIPHON SIP VOIP Client that actually compiles and runs on ios5 non-jailbroken phones. Works on the device and simulator! (GPL). Here is the original repository: http://code.google.com/p/siphon/
* [radiofreejohn/cfastread](https://github.com/radiofreejohn/cfastread) - Implementation of the Spritz reading method for command line files
* [rafael-santiago/pig](https://github.com/rafael-santiago/pig) - A Linux packet crafting tool
* [rahpaere/dc](https://github.com/rahpaere/dc) - Power grid data collector.
* [rainkid/dataserv](https://github.com/rainkid/dataserv) - dataserv
* [rajatkhanduja/Benchmarks](https://github.com/rajatkhanduja/Benchmarks) - Some programs to test the performance of two (or more) methods to achieve the same thing. It could be two (or more) data structures or two (or more) algorithms to solve the same problem
* [ramonza/libcoro](https://github.com/ramonza/libcoro) - Lightweight C coroutines (derived from http://software.schmorp.de/pkg/libcoro.html)
* [rampantpixels/foundation_lib](https://github.com/rampantpixels/foundation_lib) - Cross-platform public domain foundation library in C providing basic support data types and functions to write applications and games in a platform-independent fashion.
* [rampantpixels/rpmalloc](https://github.com/rampantpixels/rpmalloc) - Public domain cross platform lock free thread caching 32-byte aligned memory allocator implemented in C
* [randrew/layout](https://github.com/randrew/layout) - Single-file library for calculating 2D UI layouts using stacking boxes. Compiles as C99 or C++.
* [raphydaphy/Q-Operating-System](https://github.com/raphydaphy/Q-Operating-System) - Q OS is a versatile operating system designed with the new features of 64 bit "long mode" CPU's in mind that focuses on making everything as simple as possible for the end user
* [raspberrypi/maynard](https://github.com/raspberrypi/maynard) - Desktop environment for Wayland
* [raspberrypi/userland](https://github.com/raspberrypi/userland) - Source code for ARM side libraries for interfacing to Raspberry Pi GPU.
* [raspofabs/dodsrc](https://github.com/raspofabs/dodsrc) - Source for the Data-Oriented Design book
* [rathena/rathena](https://github.com/rathena/rathena) - rAthena is an open-source cross-platform MMORPG server.
* [rayh/kvo-block-binding](https://github.com/rayh/kvo-block-binding) - Use blocks to observe Objective-C properties using KVO
* [raysan5/raylib](https://github.com/raysan5/raylib) - A simple and easy-to-use library to enjoy videogames programming
* [razpeitia/data-structures](https://github.com/razpeitia/data-structures) - Stack, Queue, Binary Tree
* [rcr/rirc](https://github.com/rcr/rirc) - A terminal IRC client in C
* [rdub/smallfile](https://github.com/rdub/smallfile) - Security tool to create a large number of small (FS blocksize or less) files full of random data, in an effort to sanitize filesystem freespace and journal.
* [readium/readium-sdk](https://github.com/readium/readium-sdk) - A C++ ePub renderer SDK
* [reagent/http](https://github.com/reagent/http) - Simple HTTP client in C
* [realtalk/cve-2013-2094](https://github.com/realtalk/cve-2013-2094) - original cve-2013-2094 exploit and a rewritten version for educational purposes
* [rebol/rebol](https://github.com/rebol/rebol) - Source code for the Rebol interpreter
* [recp/cglm](https://github.com/recp/cglm) - 📽 Highly Optimized Graphics Math (glm) for C
* [redBorder/n2kafka](https://github.com/redBorder/n2kafka) - Tool that listen on a given port and throw all data received to a kafka topic
* [redbo/cloudfuse](https://github.com/redbo/cloudfuse) - Filesystem (fuse) implemented on Mosso's Cloud Files
* [redbrain/cython-book](https://github.com/redbrain/cython-book) - Learning Cython packtpub.com code examples.
* [redis/hiredis](https://github.com/redis/hiredis) - Minimalistic C client for Redis >= 1.2
* [redjack/libcork](https://github.com/redjack/libcork) - A simple, easily embeddable cross-platform C library
* [redxu/sihook](https://github.com/redxu/sihook) - source insight 3.X tabs plugin in c language
* [reeze/php-ext-embed](https://github.com/reeze/php-ext-embed) - Write your PHP extension with C and PHP!
* [regehr/ub-canaries](https://github.com/regehr/ub-canaries) - collection of C/C++ programs that try to get compilers to exploit undefined behavior
* [reicast/reicast-emulator](https://github.com/reicast/reicast-emulator) - Reicast is a multiplatform Sega Dreamcast emulator
* [remicollet/pecl-json-c](https://github.com/remicollet/pecl-json-c) - JSON-C wrapper
* [remis-thoughts/native-hdfs-fuse](https://github.com/remis-thoughts/native-hdfs-fuse) - C HDFS FUSE implementation, no libhdfs
* [rentzsch/MagicHat](https://github.com/rentzsch/MagicHat) - Objective-C Binary Documentation Tool. Think classdump with a hyperlinked GUI.
* [rentzsch/mach_inject](https://github.com/rentzsch/mach_inject) - interprocess code injection for Mac OS X
* [rentzsch/mach_star](https://github.com/rentzsch/mach_star) - code injection and function overriding for Mac OS X
* [rentzsch/markdownlive](https://github.com/rentzsch/markdownlive) - Purpose-built Markdown Editor for Mac OS X with Live Preview
* [rentzsch/stressdrive](https://github.com/rentzsch/stressdrive) - tool to completely fill a drive with random data and ensure it can be entirely correctly read back
* [reorg/pg_repack](https://github.com/reorg/pg_repack) - Reorganize tables in PostgreSQL databases with minimal locks
* [replay/ngx_http_consistent_hash](https://github.com/replay/ngx_http_consistent_hash) - a module which enables the nginx to use the same consistent hashing distribution for memcache servers as the php memcache module
* [reprappro/RepRapFirmware](https://github.com/reprappro/RepRapFirmware) - OO C++ RepRap Firmware
* [res0nat0r/tsunami-udp](https://github.com/res0nat0r/tsunami-udp) -  A fast user-space file transfer protocol that uses TCP control and UDP data for transfer over very high speed long distance networks (≥ 1 Gbps and even 10 GE), designed to provide more throughput than possible with TCP over the same networks.
* [residuum/PuRestJson](https://github.com/residuum/PuRestJson) - PuREST JSON is a library for connecting Puredata (Pd) to HTTP services  and encoding and decoding JSON data.
* [retme7/CVE-2014-4322_poc](https://github.com/retme7/CVE-2014-4322_poc) - Gain privileges:system -> root,as a part of  https://github.com/retme7/CVE-2014-7911_poc
* [retuxx/tinyspline](https://github.com/retuxx/tinyspline) - ANSI C library for NURBS, B-Splines, and Bézier curves with wrappers for C++11, C#, Java, Lua, PHP, Python, and Ruby
* [reverbrain/eblob](https://github.com/reverbrain/eblob) - Eblob is an append-only low-level IO library, which saves data in blob files. Created as low-level backend for elliptics
* [reverbrain/smack](https://github.com/reverbrain/smack) - Low-level IO storage which packs data into sorted (zlib/bzip2/snappy compressed) blobs
* [revolutionary/zergRush](https://github.com/revolutionary/zergRush) - Android 2.2 / 2.3 local root
* [rfjakob/cshatag](https://github.com/rfjakob/cshatag) - Detect silent data corruption under Linux using checksums in extended attributes
* [rfk/tnetstring](https://github.com/rfk/tnetstring) - data serialization using typed netstrings
* [rflynn/imgmin](https://github.com/rflynn/imgmin) - Lossy image optimization
* [rg3/bcrypt](https://github.com/rg3/bcrypt) - bcrypt password hash C library
* [rgantt/compsci.c](https://github.com/rgantt/compsci.c) - data structures, algorithms, and musings in C
* [rgerganov/footswitch](https://github.com/rgerganov/footswitch) - Command-line utility for PCsensor foot switch
* [rhomobile/rhodes](https://github.com/rhomobile/rhodes) - The Rhodes framework is a platform for building locally executing, device-optimized mobile applications for all major smartphone devices.
* [ricardo-rendoncepeda/mtl2opengl](https://github.com/ricardo-rendoncepeda/mtl2opengl) - A perl script for converting .obj and .mtl data files into arrays compatible with OpenGL ES on iOS devices
* [richarddurbin/pbwt](https://github.com/richarddurbin/pbwt) - Implementation of Positional Burrows-Wheeler Transform for genetic data
* [richgel999/miniz](https://github.com/richgel999/miniz) - miniz: Single C source file zlib-replacement library, originally from code.google.com/p/miniz
* [richox/comprox](https://github.com/richox/comprox) - An experimental lossless data compression program with high compression ratio.
* [ridiculousfish/cdecl-blocks](https://github.com/ridiculousfish/cdecl-blocks) - The venerable cdecl, with Apple blocks support
* [riolet/WAFer](https://github.com/riolet/WAFer) - WAFer is a C language-based software platform for scalable server-side and networking applications. Think node.js for C programmers.
* [riolet/nope.c](https://github.com/riolet/nope.c) - nope.c is a C language-based software platform for scalable server-side and networking applications. Think node.js for C programmers.
* [riolet/rix](https://github.com/riolet/rix) - Rix language combines the power of C language and the convenience of a high level language
* [rjsikarwar/gpu_compression](https://github.com/rjsikarwar/gpu_compression) - Nine Light weight Schemes to Compress and Decompress the data of Database Using GPU and also a planer
* [rmagick-temp/rmagick](https://github.com/rmagick-temp/rmagick) - An interface to the ImageMagick and GraphicsMagick image processing libraries.
* [rmccullagh/como-lang-ng](https://github.com/rmccullagh/como-lang-ng) - A programming language prototype implemented in C with an AST, Compiler, and  Virtual Machine \@TODO Garbage Collection
* [rmitton/rjm](https://github.com/rmitton/rjm) - Various single-file C libraries.
* [rmtheis/tess-two](https://github.com/rmtheis/tess-two) - Fork of Tesseract Tools for Android.
* [rnorris/viking](https://github.com/rnorris/viking) - Viking is a free/open source program to manage GPS data (including GPX and KML files). You can import and plot tracks, routes and waypoints, show OpenStreetMaps (OSM), Bing Aerial and other maps, generate Mapnik maps, geotag images, make new tracks, routes and waypoints, see real-time GPS position, etc.  It is written mostly in C with the GTK+ 2 toolkit and some C++.
* [robertdavidgraham/cve-2015-5477](https://github.com/robertdavidgraham/cve-2015-5477) - PoC exploit for CVE-2015-5477 BIND9 TKEY assertion failure
* [robertdavidgraham/heartleech](https://github.com/robertdavidgraham/heartleech) - Demonstrates the "heartbleed" problem using full OpenSSL stack
* [robertdavidgraham/isowall](https://github.com/robertdavidgraham/isowall) - This is a mini-firewall that completely isolates a target device from the local network.
* [robertdavidgraham/masscan](https://github.com/robertdavidgraham/masscan) - TCP port scanner, spews SYN packets asynchronously, scanning entire Internet in under 5 minutes.
* [robertdavidgraham/robdns](https://github.com/robertdavidgraham/robdns) - A fast DNS server based on C10M principles
* [robm/dzen](https://github.com/robm/dzen) - Dzen is a general purpose messaging, notification and menuing program for X11.
* [robmccoll/graphdb-testing](https://github.com/robmccoll/graphdb-testing) - Benchmarking various graph databases, engines, datastructures, and data stores.
* [roboterclubaachen/xpcc](https://github.com/roboterclubaachen/xpcc) - The C++ microcontroller framework xpcc for AVR and Cortex-M
* [robotmedia/RMStore](https://github.com/robotmedia/RMStore) - A lightweight iOS library for In-App Purchases
* [robotpy/robotpy-crio](https://github.com/robotpy/robotpy-crio) - Obsolete. Python 3 port for cRIO for use in the FIRST Robotics Competition (FRC)
* [robrix/RXPreprocessing](https://github.com/robrix/RXPreprocessing) - A variety of utilities for the C preprocessor.
* [robwhess/opensift](https://github.com/robwhess/opensift) - Open-Source SIFT Library
* [rockdaboot/mget](https://github.com/rockdaboot/mget) - Multithreaded metalink/file/website downloader (like Wget) and C library
* [rofl0r/libulz](https://github.com/rofl0r/libulz) - a collection of useful functions and data structures to create C apps faster. focus on simplicity, ability to statically link and minimal binary size.
* [rofl0r/proxychains-ng](https://github.com/rofl0r/proxychains-ng) - proxychains ng (new generation) - a preloader which hooks calls to sockets in dynamically linked programs and redirects it through one or more socks/http proxies. continuation of the unmaintained proxychains project.
* [romanbsd/fast-stemmer](https://github.com/romanbsd/fast-stemmer) - Fast Porter stemmer based on a C version of the algorithm
* [rothlab/chromozoom](https://github.com/rothlab/chromozoom) - ChromoZoom is a fast, fluid web-based genome browser
* [rougier/freetype-gl](https://github.com/rougier/freetype-gl) - OpenGL text using one vertex buffer, one texture and FreeType
* [roundsheep/rpp](https://github.com/roundsheep/rpp) - RPP is a new programming language combined with C++ and LISP
* [roysjosh/xbee-comm](https://github.com/roysjosh/xbee-comm) - XBee communication libraries and utilities
* [rpetrich/untrackerd](https://github.com/rpetrich/untrackerd) - Continuously clean up locationd's history data
* [rpm-software-management/hawkey](https://github.com/rpm-software-management/hawkey) - This is hawkey, library providing simplified C and Python API to libsolv. Hawkey project is obsoleted.
* [rsms/sol](https://github.com/rsms/sol) - A sunny little virtual machine
* [rspamd/rspamd](https://github.com/rspamd/rspamd) - Rapid spam filtering system.
* [rsta2/circle](https://github.com/rsta2/circle) - A C++ bare metal environment for Raspberry Pi with USB (32 and 64 bit)
* [rsta2/uspi](https://github.com/rsta2/uspi) - A bare metal USB driver for Raspberry Pi written in C
* [rswier/c4](https://github.com/rswier/c4) - C in four functions
* [rswier/swieros](https://github.com/rswier/swieros) - A tiny hand crafted CPU emulator, C compiler, and Operating System
* [rsyslog/rsyslog](https://github.com/rsyslog/rsyslog) - a Rocket-fast SYStem for LOG processing
* [rubenspessoa/LocData-P1](https://github.com/rubenspessoa/LocData-P1) - Projeto de Programação 1.
* [ruby/curses](https://github.com/ruby/curses) - Ruby binding for curses, ncurses, and PDCurses.  Formerly part of the ruby standard library.
* [ruby/psych](https://github.com/ruby/psych) - A libyaml wrapper for Ruby
* [rui314/9cc](https://github.com/rui314/9cc) - A Small C Compiler
* [rui314/minilisp](https://github.com/rui314/minilisp) - A readable lisp in less than 1k lines of C
* [rustyrussell/bitcoin-iterate](https://github.com/rustyrussell/bitcoin-iterate) - Simple fast iterator to extract data from bitcoind's blockchain files.
* [rustyrussell/ccan](https://github.com/rustyrussell/ccan) - The C Code Archive Network
* [rvoicilas/inotify-tools](https://github.com/rvoicilas/inotify-tools) -   inotify-tools is a C library and a set of command-line programs for Linux providing a simple interface to inotify.
* [rweichler/cylinder](https://github.com/rweichler/cylinder) - iOS homescreen page transitions in Lua
* [rwos/gti](https://github.com/rwos/gti) - a git launcher :-)
* [rxi/dyad](https://github.com/rxi/dyad) - Asynchronous networking for C
* [rxi/log.c](https://github.com/rxi/log.c) - A simple logging library implemented in C99
* [rxi/lovedos](https://github.com/rxi/lovedos) - A framework for making 2D DOS games in Lua
* [rxi/map](https://github.com/rxi/map) - A type-safe hash map implementation for C
* [rxi/vec](https://github.com/rxi/vec) - A type-safe dynamic array implementation for C
* [rxin/db-benchmarks](https://github.com/rxin/db-benchmarks) - Collection of some database benchmarks, along with tools to parallelize the data generation.
* [ryanb/rmov](https://github.com/ryanb/rmov) - Ruby wrapper for the QuickTime C API.
* [ryandotsmith/queue_lkls](https://github.com/ryandotsmith/queue_lkls) - A lock-free, non-blocking queue data structure.
* [ryanmjacobs/c](https://github.com/ryanmjacobs/c) - Compile and execute C "scripts" in one go!
* [ryd/chaosvpn](https://github.com/ryd/chaosvpn) - Config generator for chaos vpn
* [s-matyukevich/raspberry-pi-os](https://github.com/s-matyukevich/raspberry-pi-os) - Learning operating system development using Linux kernel and Raspberry Pi
* [s-u/iotools](https://github.com/s-u/iotools) - High-performance I/O tools to run distributed R jobs seamlessly on Hadoop and handle chunk-wise data processing
* [sackmotion/motion](https://github.com/sackmotion/motion) - Motion, a software motion detector
* [saelo/cve-2014-0038](https://github.com/saelo/cve-2014-0038) - Linux local root exploit for CVE-2014-0038
* [saghul/pycares](https://github.com/saghul/pycares) - Python interface for c-ares
* [saghul/pyuv](https://github.com/saghul/pyuv) - Python interface for libuv
* [sahib/glyr](https://github.com/sahib/glyr) - Glyr is a music related metadata searchengine, both with commandline interface and C API
* [sahib/rmlint](https://github.com/sahib/rmlint) - Extremely fast tool to remove duplicates and other lint from your filesystem
* [sainteos/tmxparser](https://github.com/sainteos/tmxparser) - C++ library for parsing the maps generated by the Map Editor called Tiled.
* [samdeane/xcode-unicode-formatter](https://github.com/samdeane/xcode-unicode-formatter) - Xcode data view plugin for formatting 16-bit and 32-bit unicode strings
* [samdmarshall/SDMMobileDevice](https://github.com/samdmarshall/SDMMobileDevice) - MobileDevice Implementation
* [samop/Polar-Flowlink-linux](https://github.com/samop/Polar-Flowlink-linux) - Development of interface for Polar FT60 HRM for Linux. It was tested with FT80 and it didn't work, due to different command set. I will need physical access to the watch to be able to devise a solution for other HRMs. Simple one page web interface that can be run on local machine and mimics polarpersonaltrainer is also included (see screenshot) but needs lots of polishing. Please note it is a work in progress. This early version pulls down all data except for weekly training program.
* [samrushing/irken-compiler](https://github.com/samrushing/irken-compiler) - Irken is a statically typed variant of Scheme.  Or a lisp-like variant of ML.
* [samtools/htslib](https://github.com/samtools/htslib) - C library for high-throughput sequencing data formats
* [samtools/samtools](https://github.com/samtools/samtools) - Tools (written in C using htslib) for manipulating next-generation sequencing data
* [samuellab/InterProcess](https://github.com/samuellab/InterProcess) - A compact C library to share data between processes on Windows. Fast. Simple
* [samyk/pwnat](https://github.com/samyk/pwnat) - pwnat punches holes in firewalls and NATs allowing any numbers of clients behind NATs to directly connect to a server behind a different NAT with no 3rd party, port forwarding, DMZ or spoofing involved
* [saprykin/plibsys](https://github.com/saprykin/plibsys) - Highly portable C system library: threads and synchronization primitives, sockets (TCP, UDP, SCTP), IPv4 and IPv6, IPC, hash functions (MD5, SHA-1, SHA-2, SHA-3, GOST), binary trees (RB, AVL) and more. Native code performance.
* [sass/sassc](https://github.com/sass/sassc) - libsass command line driver
* [satellogic/canopus](https://github.com/satellogic/canopus) - Canopus framework and flight computer software for CubeBug cubesat platform
* [sbinet/go-clang](https://github.com/sbinet/go-clang) - CGo bindings to the C-api of libclang.
* [scallopedllama/nerorip](https://github.com/scallopedllama/nerorip) - Rips data out of nero archives
* [sch3m4/libntoh](https://github.com/sch3m4/libntoh) - User-friendly C Library to perform TCP streams reassembly and IPv4/6 defragmentation
* [schweikert/fping](https://github.com/schweikert/fping) - High performance ping tool
* [sciguy14/MSP430-Wireless-Weather-Station](https://github.com/sciguy14/MSP430-Wireless-Weather-Station) - A Remote MSP430 monitors temperature, light, and humidity and sends the data to a local UART-USB MSP430.  A processing script graphs the data in real time on a computer.
* [scottcgi/Mojoc](https://github.com/scottcgi/Mojoc) - A cross-platform, open-source, pure C  game engine for mobile game.
* [scottellis/snapx](https://github.com/scottellis/snapx) - Stream data from a v4l2 camera and periodically save image. Testing app.
* [scottransom/psrfits2psrfits](https://github.com/scottransom/psrfits2psrfits) - Convert 16-bit PSRFITS search-mode data to 4- or 8-bit PSRFITS data
* [scrapinghub/mdr](https://github.com/scrapinghub/mdr) - A python library detect and extract listing data from HTML page.
* [scytulip/nrf51-back-rec](https://github.com/scytulip/nrf51-back-rec) - NRF51822 Firmware for Background Data Recording
* [sdegutis/mjolnir](https://github.com/sdegutis/mjolnir) - Lightweight automation and productivity app for OS X
* [sdhand/x11fs](https://github.com/sdhand/x11fs) - A tool for manipulating X windows
* [sdiehl/pycraig](https://github.com/sdiehl/pycraig) - Python library for scraping data from Craigslist
* [sdroege/snippets](https://github.com/sdroege/snippets) - Some algorithms and data structures
* [seL4/seL4](https://github.com/seL4/seL4) - The seL4 microkernel
* [sean-/postgresql-varint](https://github.com/sean-/postgresql-varint) - Data type for PostgreSQL that encodes integers using variable width encoding in order to save space
* [seanmiddleditch/libtelnet](https://github.com/seanmiddleditch/libtelnet) - Simple RFC-complient TELNET implementation as a C library.
* [seanooi/iOS-WebP](https://github.com/seanooi/iOS-WebP) - Google's WebP image format decoder and encoder for iOS
* [searchdaimon/enterprise-search](https://github.com/searchdaimon/enterprise-search) - An open source search engine for corporate data and websites.
* [seastorm/PuttyRider](https://github.com/seastorm/PuttyRider) - Hijack Putty sessions in order to sniff conversation and inject Linux commands.
* [sebnow/data_structures](https://github.com/sebnow/data_structures) - A collection of data structures, written in C.
* [seemoo-lab/nexmon](https://github.com/seemoo-lab/nexmon) - The C-based Firmware Patching Framework for Broadcom/Cypress WiFi Chips that enables Monitor Mode, Frame Injection and much more
* [seenaburns/stag](https://github.com/seenaburns/stag) - Streaming bar graphs. For stats and stuff.
* [sektioneins/SUIDGuard](https://github.com/sektioneins/SUIDGuard) - SUIDGuard - a TrustedBSD Kernel Extension that adds mitigations to protect SUID/SGID processes a bit more
* [selkhateeb/hardlink](https://github.com/selkhateeb/hardlink) - a simple command-line utility that implements hardlinks on Mac OsX
* [semmerson/NOAAPORT](https://github.com/semmerson/NOAAPORT) - The Unidata NOAAPORT package captures broadcast UDP packets from a DVB-S or DVB-S2 receiver listening to the NOAAPORT satellite broadcast, creates data-products from the UDP packets, and inserts those data-products into an LDM product-queue.
* [seppo0010/rlite](https://github.com/seppo0010/rlite) - self-contained, serverless, zero-configuration, transactional redis-compatible database engine. rlite is to Redis what SQLite is to SQL.
* [septag/darkhammer](https://github.com/septag/darkhammer) - darkHAMMER is a lightweight, open-source, multiplatform game engine. written in C (C99) language, supports python and C# bindings and lua scripts. Runs on windows and linux
* [servalproject/batphone](https://github.com/servalproject/batphone) - The Serval Mesh app for Android.  EXPERIMENTAL SOFTWARE.
* [session-replay-tools/tcpburn](https://github.com/session-replay-tools/tcpburn) - The most powerful tool for stress testing of Internet server applications
* [session-replay-tools/tcpcopy](https://github.com/session-replay-tools/tcpcopy) - An online request replication tool, also a tcp stream replay tool, fit for real testing, performance testing, stability testing, stress testing, load testing, smoke testing, etc
* [seth/crio](https://github.com/seth/crio) - Prototype R package providing C-level utils for streaming data processing
* [seth/rdict](https://github.com/seth/rdict) - R dictionary data type
* [sevenler/Uninstall_Statics](https://github.com/sevenler/Uninstall_Statics) - Android 统计 应用 自身被 卸载 Android Statistics application is uninstalled
* [sgminer-dev/sgminer](https://github.com/sgminer-dev/sgminer) - Scrypt GPU miner
* [shadeslayer/libnice](https://github.com/shadeslayer/libnice) - Libnice is an implementation of the IETF's Interactive Connectivity Establishment (ICE) standard (RFC 5245) and the Session Traversal Utilities for NAT (STUN) standard (RFC 5389).  It provides a GLib-based library, libnice and a Glib-free library, libstun as well as GStreamer elements.  ICE is useful for applications that want to establish peer-to-peer UDP data streams. It automates the process of traversing NATs and provides security against some attacks. It also allows applications to create reliable streams using a TCP over UDP layer.  Existing standards that use ICE include Session Initiation Protocol (SIP) and XMPP Jingle.
* [shadowsocks/ChinaDNS](https://github.com/shadowsocks/ChinaDNS) - Protect yourself against DNS poisoning in China.
* [shadowsocks/shadowsocks-android](https://github.com/shadowsocks/shadowsocks-android) - A Shadowsocks client for Android
* [shannah/Java-Objective-C-Bridge](https://github.com/shannah/Java-Objective-C-Bridge) - A thin bridge that allows for two-way communication from Java to Objective-C.
* [shantzu/ClipIt](https://github.com/shantzu/ClipIt) - ClipIt clipboard manager for GTK+
* [sharelatex/clsi-sharelatex](https://github.com/sharelatex/clsi-sharelatex) - A web api for compiling LaTeX documents in the cloud
* [sharvil/flingfd](https://github.com/sharvil/flingfd) - A tiny library to send file descriptors across processes
* [shaunlebron/blinky](https://github.com/shaunlebron/blinky) - Exploring peripheral vision in games (using Quake)
* [shawnclovie/cocos2dx-LuaProxy](https://github.com/shawnclovie/cocos2dx-LuaProxy) - LuaProxy for cocos2d-x, include CocosBuilder support for lua, and other cocos2d-extension support for lua, and easy to use function.
* [sheepdog/sheepdog](https://github.com/sheepdog/sheepdog) - Distributed Storage System for QEMU
* [shenfeng/tiny-web-server](https://github.com/shenfeng/tiny-web-server) - a tiny web server in C, for daily use.
* [sheredom/json.h](https://github.com/sheredom/json.h) - json parser for C and C++
* [sheredom/process.h](https://github.com/sheredom/process.h) - A simple one header solution to launching processes and interacting with them for C and C++.
* [sheredom/utf8.h](https://github.com/sheredom/utf8.h) - single header utf8 string functions for C and C++
* [shinh/maloader](https://github.com/shinh/maloader) - mach-o loader for linux
* [shiziwen/nagios-status2txt](https://github.com/shiziwen/nagios-status2txt) - nagios enhancement to get service data as plain text
* [shoes/shoes](https://github.com/shoes/shoes) - a tiny graphical app kit for ruby
* [shtrom/xkeyboard-config](https://github.com/shtrom/xkeyboard-config) - Mirror of FreeDesktop.org's XKB data with local branches
* [shuLhan/vos](https://github.com/shuLhan/vos) - Vos is a program to process formatted data, i.e. CSV data. Vos is designed to process a large input file, a file where their size is larger than the size of memory, and can be tuned to adapt with your machine environment.
* [sickill/stderred](https://github.com/sickill/stderred) - stderr in red
* [siddhant3s/cs215](https://github.com/siddhant3s/cs215) - My Third Semester, Data Structure Lab programs
* [siddontang/libtnet](https://github.com/siddontang/libtnet) - libtnet is a tiny high performance c++ network lib, like tornado
* [siemens/jailhouse](https://github.com/siemens/jailhouse) - Linux-based partitioning hypervisor
* [siganakis/tny](https://github.com/siganakis/tny) - Tiny data structures that pack a punch!
* [signal11/hidapi](https://github.com/signal11/hidapi) - A Simple library for communicating with USB and Bluetooth HID devices on Linux, Mac, and Windows.
* [signalapp/libsignal-protocol-c](https://github.com/signalapp/libsignal-protocol-c) - Signal Protocol C Library
* [silentbicycle/greatest](https://github.com/silentbicycle/greatest) - A C testing library in 1 file. No dependencies, no dynamic allocation. ISC licensed.
* [silentbicycle/theft](https://github.com/silentbicycle/theft) - property-based testing for C: generate input to find obscure bugs, then reduce to minimal failing input
* [simondlevy/BreezySLAM](https://github.com/simondlevy/BreezySLAM) - Simple, efficient, open-source package for Simultaneous Localization and Mapping in Python, Matlab,  Java, and C++
* [simondlevy/TinyEKF](https://github.com/simondlevy/TinyEKF) - Lightweight C/C++ Extended Kalman Filter with Python for prototyping
* [simonyiszk/csdr](https://github.com/simonyiszk/csdr) - A simple DSP library and command-line tool for Software Defined Radio.
* [simpl/ngx_devel_kit](https://github.com/simpl/ngx_devel_kit) - Nginx Development Kit - an Nginx module that adds additional generic tools that module developers can use in their own modules
* [simple2d/simple2d](https://github.com/simple2d/simple2d) - :video_game: Simple, open-source 2D graphics for everyone
* [simplegeo/libgeohash](https://github.com/simplegeo/libgeohash) - A pure C implementation of the Geohash algorithm.
* [simtr/The-Powder-Toy](https://github.com/simtr/The-Powder-Toy) - Written in C++ and using SDL, The Powder Toy is a desktop version of the classic 'falling sand' physics sandbox, it simulates air pressure and velocity as well as heat.
* [sipcapture/hepipe](https://github.com/sipcapture/hepipe) - HEP-PIPE: Pipe arbitrary data (logs, events, cdrs, etc) to HEP server (HOMER)
* [sisong/HDiffPatch](https://github.com/sisong/HDiffPatch) - a C\C++ library and command-line tools for binary data Diff & Patch; fast and create small delta/differential; support large files and limit memory requires when diff&patch.
* [siu/minunit](https://github.com/siu/minunit) - Minimal unit testing framework for C
* [sixstars/CTF](https://github.com/sixstars/CTF) - A writeup summary for CTF competitions, problems.
* [sixstars/ctf](https://github.com/sixstars/ctf) - A writeup summary for CTF competitions, problems.
* [skarnet/s6](https://github.com/skarnet/s6) - The s6 supervision suite.
* [skeeto/interactive-c-demo](https://github.com/skeeto/interactive-c-demo) - Demonstration of interactive C programming
* [skopjehacklab/MeteoKutija](https://github.com/skopjehacklab/MeteoKutija) - The MeteoBox (MeteoKutija) is a cheap device that collects a set of meteorological data and publishes it to a central database.
* [skvadrik/re2c](https://github.com/skvadrik/re2c) - lexer generator for C/C++
* [skx/simple.vm](https://github.com/skx/simple.vm) - Simple virtual machine which inteprets bytecode.
* [slact/nginx_http_push_module](https://github.com/slact/nginx_http_push_module) - Turn NGiNX into an adept HTTP push server.
* [slash-lang/slash](https://github.com/slash-lang/slash) - A new language for the web
* [slembcke/Chipmunk2D](https://github.com/slembcke/Chipmunk2D) - A fast and lightweight 2D game physics library.
* [sleuthkit/sleuthkit](https://github.com/sleuthkit/sleuthkit) - The Sleuth Kit® (TSK) is a library and collection of command line digital forensics tools that allow you to investigate volume and file system data. The library can be incorporated into larger digital forensics tools and the command line tools can be directly used to find evidence.
* [slim-curve/slim-curve](https://github.com/slim-curve/slim-curve) - SLIM Curve: a package for exponential curve fitting of combined spectral lifetime image data
* [smealum/ctrulib](https://github.com/smealum/ctrulib) - C library for writing user mode arm11 code for the 3DS (CTR)
* [smira/memcached_functions_mysql](https://github.com/smira/memcached_functions_mysql) - Memcached functions for MySQL as UDF, tailored for usage in replication and pushing data to MemcacheQ
* [smistad/GPU-Marching-Cubes](https://github.com/smistad/GPU-Marching-Cubes) - A GPU implementation of the Marching Cubes algorithm for extracting surfaces from volumes using OpenCL and OpenGL
* [smithlabcode/methpipe](https://github.com/smithlabcode/methpipe) - A pipeline for analyzing DNA methylation data from bisulfite sequencing.
* [smtlaissezfaire/c_type_sizes](https://github.com/smtlaissezfaire/c_type_sizes) - show the sizes of C data types
* [snaga/monetdb_fdw](https://github.com/snaga/monetdb_fdw) - monetdb_fdw - PostgreSQL Foreign Data Wrapper for MonetDB
* [snaga/xlogdump](https://github.com/snaga/xlogdump) - A tool for extracting data from the PostgreSQL's write ahead logs.
* [snavely/bundler_sfm](https://github.com/snavely/bundler_sfm) - Bundler Structure from Motion Toolkit
* [snielsen/DeathToDSStore](https://github.com/snielsen/DeathToDSStore) - .DS_Store is an abomination and must be stopped.
* [snooda/net-speeder](https://github.com/snooda/net-speeder) - net-speeder 在高延迟不稳定链路上优化单线程下载速度
* [solusipse/ureq](https://github.com/solusipse/ureq) - Micro C library for handling HTTP requests on low resource systems.
* [sonsongithub/CoreAR](https://github.com/sonsongithub/CoreAR) - AR(Augmented reality) framework for iOS, based on a visual code like ARToolKit
* [sonyxperiadev/kernel-copyleft](https://github.com/sonyxperiadev/kernel-copyleft) - Copyleft archives for Xperia kernels
* [sounos/hidbase](https://github.com/sounos/hidbase) - Distributed Data Storage System
* [soveran/clac](https://github.com/soveran/clac) - Command-line, stack-based calculator with postfix notation
* [sp4cerat/RLE-based-Voxel-Raycasting](https://github.com/sp4cerat/RLE-based-Voxel-Raycasting) - CUDA based Voxel Raycasting - Paper: Efficient, High-Quality, GPU-Based Visualization of Voxelized Surface Data
* [spark/core-common-lib](https://github.com/spark/core-common-lib) - Common library for projects that use the Spark Core with the CC3000
* [spark/firmware](https://github.com/spark/firmware) - Firmware for Particle Devices
* [sphde/sphde](https://github.com/sphde/sphde) - Shared Persistent Heap Data Environment
* [spotify/sparkey](https://github.com/spotify/sparkey) - Simple constant key/value storage library, for read-heavy systems with infrequent large bulk inserts.
* [sptim/mp3hash](https://github.com/sptim/mp3hash) - Command line tool to calculate the hash of the music data in mp3 files (without id3v1 & id3v2 metadata). Useful to find dupes with e.g. different genre names.
* [sqlcipher/sqlcipher](https://github.com/sqlcipher/sqlcipher) - SQLCipher is an SQLite extension that provides 256 bit AES encryption of database files.
* [squix78/esp8266-weather-station-color](https://github.com/squix78/esp8266-weather-station-color) - ESP8266 Weather Station in Color using ILI9341 TFT 240x320 display
* [srdja/Collections-C](https://github.com/srdja/Collections-C) - A library of generic data structures.
* [srijs/udp-stats-redis-adapter](https://github.com/srijs/udp-stats-redis-adapter) - Small performant frontend to redis, receiving minimal statistics data via udp messaging.
* [ssfrr/HearThereOSC](https://github.com/ssfrr/HearThereOSC) - A small program to receive some IMU orientation data from the HearThere Head Tracker
* [sshirokov/csgtool](https://github.com/sshirokov/csgtool) - 3D CSG Tool
* [st3fan/ios-openssl](https://github.com/st3fan/ios-openssl) - Port of OpenSSL for iOS
* [starnight/simple-data-structure](https://github.com/starnight/simple-data-structure) - Simple Data Structure library
* [statsite/statsite](https://github.com/statsite/statsite) - C implementation of statsd
* [stawel/cheali-charger](https://github.com/stawel/cheali-charger) - cheap lipo charger
* [steakknife/unsign](https://github.com/steakknife/unsign) - Remove code signatures from OSX Mach-O binaries (note: unsigned binaries cannot currently be re-codesign'ed. Patches welcome!)
* [stec-inc/EnhanceIO](https://github.com/stec-inc/EnhanceIO) - EnhanceIO Open Source for Linux
* [stedolan/jq](https://github.com/stedolan/jq) - Command-line JSON processor
* [stefanesser/dumpdecrypted](https://github.com/stefanesser/dumpdecrypted) - Dumps decrypted mach-o files from encrypted iPhone applications from memory to disk. This tool is necessary for security researchers to be able to look under the hood of encryption.
* [stefanesser/suhosin](https://github.com/stefanesser/suhosin) - Suhosin Extension
* [stefanhafeneger/PushMeBaby](https://github.com/stefanhafeneger/PushMeBaby) - iOS Push Notification Debug App
* [stellar/stellar-core](https://github.com/stellar/stellar-core) - stellar-core is the backbone of the Stellar network. It maintains a local copy of the ledger, communicating and staying in sync with other instances of stellar-core on the network. Optionally, stellar-core can store historical records of the ledger and participate in consensus.
* [stellarscience/xdm](https://github.com/stellarscience/xdm) - An Extensible Data Model
* [stephane/libmodbus](https://github.com/stephane/libmodbus) - A Modbus library for Linux, Mac OS X, FreeBSD, QNX and Windows
* [stephenmathieson/describe.h](https://github.com/stephenmathieson/describe.h) - Simple BDD describe test thingy for C
* [stephenrkell/liballocs](https://github.com/stephenrkell/liballocs) - Runtime and toolchain for whole-program monitoring of allocations and their data types
* [stepmania/stepmania](https://github.com/stepmania/stepmania) - Advanced rhythm game for Windows, Linux and OS X. Designed for both home and arcade use.
* [stevedekorte/basekit](https://github.com/stevedekorte/basekit) - C based OO portable data structure library
* [stevedekorte/coroutine](https://github.com/stevedekorte/coroutine) - C multiplatform coroutine implementation via ucontext, fibers or setjmp.
* [stevedekorte/garbagecollector](https://github.com/stevedekorte/garbagecollector) - Incrementall garbage collector library in C for use by high level language implementions.
* [stevedekorte/io](https://github.com/stevedekorte/io) - Io programming language
* [stevedekorte/skipdb](https://github.com/stevedekorte/skipdb) - C based ordered key-value ACID DB using skiplist datastructure.
* [stevedekorte/vertexdb](https://github.com/stevedekorte/vertexdb) - C graph db server using tokyocabinet & libevent
* [steven-schronk/C-Data-Structures](https://github.com/steven-schronk/C-Data-Structures) - Collection of basic data structures in C.
* [stevestreza/CrashReporter](https://github.com/stevestreza/CrashReporter) - Send iOS crash reports by email
* [stm32duino/Arduino_Core_STM32](https://github.com/stm32duino/Arduino_Core_STM32) - STM32 core support for Arduino
* [strands-project/data_compression](https://github.com/strands-project/data_compression) - Video encoding for 8 bit RGB images, 16 bit grayscale depth images and possibly more.
* [strazzere/android-unpacker](https://github.com/strazzere/android-unpacker) - Android Unpacker presented at Defcon 22: Android Hacker Protection Level 0
* [stripydog/kplex](https://github.com/stripydog/kplex) - kplex marine data multiplexer
* [stubma/WiEngine](https://github.com/stubma/WiEngine) - C++ implemented, cocos2d like cross-platform game engine
* [studio-ousia/mprpc](https://github.com/studio-ousia/mprpc) - A fast MessagePack RPC library
* [styxyang/dnsmasq-chinadns](https://github.com/styxyang/dnsmasq-chinadns) - A patched version of dnsmasq which filters out some spurious IP
* [sufficientlysecure/ad-away](https://github.com/sufficientlysecure/ad-away) - AdAway is an open source ad blocker for Android using the hosts file.
* [suhetao/stm32f4_mpu9250](https://github.com/suhetao/stm32f4_mpu9250) - Access the data of 3-axis magnetometer and DMP from MPU9250 with SPI interface, All data fusion via EKF/UKF/CKF/SRCKF algorithm
* [sumatrapdfreader/sumatrapdf](https://github.com/sumatrapdfreader/sumatrapdf) - SumatraPDF reader
* [supertunaman/cdl](https://github.com/supertunaman/cdl) - Chicken Dance License! The official IANAL license.
* [suprgyabhushan/Data-Structures-And-Algorithms](https://github.com/suprgyabhushan/Data-Structures-And-Algorithms) - All my codes done in the Course DSA during the second semester at IIIT Bangalore
* [sustrik/libdill](https://github.com/sustrik/libdill) - Structured concurrency in C
* [sustrik/libmill](https://github.com/sustrik/libmill) - Go-style concurrency in C
* [sustrik/msg_control](https://github.com/sustrik/msg_control) - Helper functions for dealing with socket ancillary data
* [suzukiplan/Touhou-VGS-MML-data](https://github.com/suzukiplan/Touhou-VGS-MML-data) - 東方BGM on VGSのMMLデータ公開＆サポート用のレポジトリです
* [svanderburg/libamivideo](https://github.com/svanderburg/libamivideo) - Conversion library for Amiga planar graphics data and EHB, HAM screen modes
* [swatkat/twitcurl](https://github.com/swatkat/twitcurl) - twitcurl is a pure C++ library for twitter APIs.
* [swenson/sort](https://github.com/swenson/sort) - Sorting routine implementations in "template" C
* [swetland/dcpu16](https://github.com/swetland/dcpu16) - Virtual Machine and Assembler for Notch's DCPU-16 Architecture
* [switchbrew/libnx](https://github.com/switchbrew/libnx) - Library for Switch Homebrew
* [swoole/php-cp](https://github.com/swoole/php-cp) - pdo and redis tcp connect proxy
* [swoole/swoole-src](https://github.com/swoole/swoole-src) - Asynchronous & concurrent & distributed networking framework for PHP.
* [symisc/PH7](https://github.com/symisc/PH7) - An Embedded Implementation of PHP (C Library)
* [symisc/sod](https://github.com/symisc/sod) - An Embedded Computer Vision & Machine Learning Library (CPU Optimized & IoT Capable)
* [symisc/unqlite](https://github.com/symisc/unqlite) - An Embedded NoSQL, Transactional Database Engine
* [symisc/vedis](https://github.com/symisc/vedis) - An Embedded Implementation of Redis
* [synergy/synergy](https://github.com/synergy/synergy) - Share one mouse and keyboard between multiple computers on your desk.
* [synthetos/TinyG](https://github.com/synthetos/TinyG) - Affordable Industrial Grade Motion Control
* [syoyo/tinygltfloader](https://github.com/syoyo/tinygltfloader) - Header only C++ Tiny glTF loader.
* [sysstat/sysstat](https://github.com/sysstat/sysstat) - Performance monitoring tools for Linux
* [systemd/casync](https://github.com/systemd/casync) - Content-Addressable Data Synchronization Tool
* [systemd/systemd](https://github.com/systemd/systemd) - The systemd System and Service Manager
* [syuhari/cocos2dx_recipe](https://github.com/syuhari/cocos2dx_recipe) - Cocos2d-x 開発のレシピのサンプルコード
* [sztupy/luadec51](https://github.com/sztupy/luadec51) - Lua Decompiler for Lua version 5.1
* [tadasv/csv_parser](https://github.com/tadasv/csv_parser) - Callback based (SAX like) CSV Parser for C
* [taf2/curb](https://github.com/taf2/curb) - Ruby bindings for libcurl
* [taf2/libebb](https://github.com/taf2/libebb) - a lightweight high-performance HTTP server library for C
* [tai/ruby-p-for-c](https://github.com/tai/ruby-p-for-c) - Data dumper macro for C, which dumps content of any data/structure/expression without prior knowledge of actual format. Works just like "p" or "pp" in Ruby.
* [tailhook/objpath](https://github.com/tailhook/objpath) - A library that allows to traverse data structures by path
* [tailhook/zerogw](https://github.com/tailhook/zerogw) - A fast HTTP/WebSocket to zeromq gateway
* [takev/mod_okioki](https://github.com/takev/mod_okioki) - An apache module that offers a RESTful data service with a PostgresQL server.
* [tallsam/DAFWAWeatherWatch](https://github.com/tallsam/DAFWAWeatherWatch) - Pebble watch face using dafwa weather api data.
* [tanakh/cmdline](https://github.com/tanakh/cmdline) - A Command Line Parser
* [tang3w/CocoaSugar](https://github.com/tang3w/CocoaSugar) - Some Cocoa Touch improvements can make developing apps easier
* [taogogo/geohash-php-extention](https://github.com/taogogo/geohash-php-extention) - a php extension for geohash,geohash is writen in c,very fast to convert geohash and coord.(一个转换经纬度和geohash的PHP扩展)
* [tarantool/tarantool](https://github.com/tarantool/tarantool) - Get your data in RAM. Get compute close to data. Enjoy the performance.
* [tarcieri/cool.io](https://github.com/tarcieri/cool.io) - Simple evented I/O for Ruby (but please check out Celluloid::IO instead)
* [tarequeh/DES](https://github.com/tarequeh/DES) - Implementation of Data Encryption Standard (DES) in C
* [tass-belgium/picotcp](https://github.com/tass-belgium/picotcp) - PicoTCP is a free TCP/IP stack implementation
* [tatsuhiro-t/nghttp2](https://github.com/tatsuhiro-t/nghttp2) - nghttp2 - HTTP/2 C Library
* [tatsuhiro-t/spdylay](https://github.com/tatsuhiro-t/spdylay) - The experimental SPDY protocol version 2, 3 and 3.1 implementation in C
* [tatsuhiro-t/wslay](https://github.com/tatsuhiro-t/wslay) - The WebSocket library in C
* [taviso/ctypes.sh](https://github.com/taviso/ctypes.sh) - A foreign function interface for bash.
* [taylor001/crown](https://github.com/taylor001/crown) - The flexible game engine.
* [tbeu/ExternData](https://github.com/tbeu/ExternData) - :page_facing_up: Modelica library for reading data from INI, JSON, XML and Excel XLS files
* [tboox/tbox](https://github.com/tboox/tbox) - 🎁 A glib-like multi-platform c library
* [tbuktu/libntru](https://github.com/tbuktu/libntru) - C Implementation of NTRUEncrypt
* [tcbrindle/raytracer.hpp](https://github.com/tcbrindle/raytracer.hpp) - Simple compile-time raytracer using C++17
* [tcurdt/iProxy](https://github.com/tcurdt/iProxy) - Let's you connect your laptop to the iPhone to surf the web.
* [teachop/FlexCAN_Library](https://github.com/teachop/FlexCAN_Library) - Arduino library for CAN on Teensy 3.1
* [teamBICYCLE/libdatac](https://github.com/teamBICYCLE/libdatac) - a collection of data library
* [tedluo/rs485](https://github.com/tedluo/rs485) - This is a simple drive for rs485 to translate data between two arm 6410 openboard
* [tekknolagi/carp](https://github.com/tekknolagi/carp) - "interesting" VM in C. Let's see how this goes.
* [telehash/telehash-c](https://github.com/telehash/telehash-c) - telehash tools library in c
* [teletautala/fullypwnd](https://github.com/teletautala/fullypwnd) - This program is designed to identify operating system and running services and find exploits for those services and attempt to connect.  I wanted that when the program finishes it's scan there was a way to report, annotate and clarify data.
* [tenderlove/psych](https://github.com/tenderlove/psych) - A libyaml wrapper for Ruby
* [texane/stlink](https://github.com/texane/stlink) - stm32 discovery line linux programmer
* [tfoldi/fuse-tableaufs](https://github.com/tfoldi/fuse-tableaufs) - User-space filesystem for Tableau Server for accessing workbooks and data sources as files.
* [tglman/orientdb-c](https://github.com/tglman/orientdb-c) - The C client of  OrientDB
* [the-tcpdump-group/libpcap](https://github.com/the-tcpdump-group/libpcap) - the LIBpcap interface to various kernel packet capture mechanism
* [the-tcpdump-group/tcpdump](https://github.com/the-tcpdump-group/tcpdump) - the TCPdump network dissector
* [theKeithD/thmj3g-tools](https://github.com/theKeithD/thmj3g-tools) - Collection of tools to unpack and repack data used by the D.N.A.Softwares doujin game, Touhou Unreal Mahjong 3rd Generation.
* [theck01/offbrand_lib](https://github.com/theck01/offbrand_lib) - A collecton of generic reference counted data structures, tools to create compatible C style classes, and demo applications
* [thegenemyers/DAZZ_DB](https://github.com/thegenemyers/DAZZ_DB) - The Dazzler Data Base
* [thegenemyers/DEXTRACTOR](https://github.com/thegenemyers/DEXTRACTOR) - Bax File Decoder and Data Compressor
* [theunamedguy/market-sim](https://github.com/theunamedguy/market-sim) - A retro stock-trading game utilizing live market data
* [thlorenz/learnuv](https://github.com/thlorenz/learnuv) - Learn uv for fun and profit, a self guided workshop to the library that powers Node.js.
* [thomasbhatia/nwEPC---EPC-SAE-Gateway](https://github.com/thomasbhatia/nwEPC---EPC-SAE-Gateway) - nwEPC is a free and open source framework software implementation of SAE/EPC Serving Gateway or SGW and Packet Data Network Gateway or PGW, which is sometimes referred as SAE-Gateway as well.
* [thomasdenney/ObjectiveGumbo](https://github.com/thomasdenney/ObjectiveGumbo) - An Objective-C wrapper with utility functions around Gumbo for easy HTML5 parsing in Cocoa and Cocoa Touch
* [thoughtbot/pick](https://github.com/thoughtbot/pick) - fuzzy select anything.
* [thunisoft/unispim](https://github.com/thunisoft/unispim) - 华宇拼音输入法核心源码(source code of unispim)
* [thvdburgt/KnR-The-C-Programming-Language-Solutions](https://github.com/thvdburgt/KnR-The-C-Programming-Language-Solutions) - My solutions to the exercises in the book "The C Programming Language" (2nd edition) by Brian W. Kernighan and Dennis M. Ritchie, also referred to as K&R.
* [tiancaiamao/datastruct](https://github.com/tiancaiamao/datastruct) - some useful data struct piece of code
* [tiancaiamao/go-internals](https://github.com/tiancaiamao/go-internals) - dig into implemention of the go programming language
* [tianocore/edk2](https://github.com/tianocore/edk2) - EDK II
* [tianyaqu/mongodb-in-financial-market](https://github.com/tianyaqu/mongodb-in-financial-market) - mongodb solution for financial market data
* [tiehuis/2048-cli](https://github.com/tiehuis/2048-cli) - The game 2048 for your Linux terminal (https://github.com/gabrielecirulli/2048)
* [tiglabs/containerdns](https://github.com/tiglabs/containerdns) - a full cache DNS for kubernetes
* [tilgovi/couchdb-lounge](https://github.com/tilgovi/couchdb-lounge) - The Lounge is a proxy-based partitioning/clustering framework for CouchDB
* [timburks/NuMongoDB](https://github.com/timburks/NuMongoDB) - An Objective-C interface to MongoDB for use with Nu
* [timperrett/Mac-SoapClient](https://github.com/timperrett/Mac-SoapClient) - 10.7 Compatible version of this: http://code.google.com/p/mac-soapclient/
* [timwr/CVE-2014-3153](https://github.com/timwr/CVE-2014-3153) - CVE-2014-3153 aka towelroot
* [timwr/CVE-2016-5195](https://github.com/timwr/CVE-2016-5195) - CVE-2016-5195 (dirtycow/dirtyc0w) proof of concept for Android
* [tinyalsa/tinyalsa](https://github.com/tinyalsa/tinyalsa) - Tiny library to interface with ALSA in the Linux kernel
* [tizian/Cendric2](https://github.com/tizian/Cendric2) - 2D Game
* [tj/histo](https://github.com/tj/histo) - beautiful charts in the terminal for static or streaming data
* [tj/luna](https://github.com/tj/luna) - luna programming language - a small, elegant VM implemented in C
* [tj/mon](https://github.com/tj/mon) - mon(1) - Simple single-process process monitoring program written in C
* [tj/watch](https://github.com/tj/watch) - watch(1) periodically executes the given command - useful for auto-testing, auto-building, auto-anything
* [tj90241/cen64](https://github.com/tj90241/cen64) - Cycle-Accurate Nintendo 64 Emulator
* [tjko/jpegoptim](https://github.com/tjko/jpegoptim) - jpegoptim - utility to optimize/compress JPEG files
* [tmk/tmk_keyboard](https://github.com/tmk/tmk_keyboard) - keyboard controller firmware for Atmel AVR USB family
* [tmm1/gctools](https://github.com/tmm1/gctools) - profiler/logger/oobgc for rgengc in ruby 2.1
* [tmm1/pygments.rb](https://github.com/tmm1/pygments.rb) - pygments syntax highlighting in ruby
* [tmm1/rblineprof](https://github.com/tmm1/rblineprof) - line-profiler for ruby
* [tmux/tmux](https://github.com/tmux/tmux) - tmux source code
* [tnightingale/DTE](https://github.com/tnightingale/DTE) - Dumb Terminal Emulator - Data Comm, COMP 3980
* [tnm/vulcan](https://github.com/tnm/vulcan) - Generate test data for Redis
* [todace/G-CVSNT](https://github.com/todace/G-CVSNT) - G-CVSNT Gaijin (and Gamedev) CVSNT version - modified for large amounts of binary data (typically for gamedev)
* [todbot/arduino-serial](https://github.com/todbot/arduino-serial) - Example C and Java host code to talking to an arduino or other "serial" device
* [toddtreece/lib_mysqludf_mongodb](https://github.com/toddtreece/lib_mysqludf_mongodb) - MySQL UDF for inserting data into MongoDB
* [tokuhirom/shirokaned](https://github.com/tokuhirom/shirokaned) - simple cache server for small binary data, feed contents with http protocol, master-master support.
* [toland/patron](https://github.com/toland/patron) - Ruby HTTP client based on libcurl
* [toland/qlmarkdown](https://github.com/toland/qlmarkdown) - QuickLook generator for Markdown files.
* [tomxue/spi](https://github.com/tomxue/spi) - to show to make SPI data transfer under Linux
* [tonyrog/cl](https://github.com/tonyrog/cl) - OpenCL binding for Erlang
* [topameng/CsToLua](https://github.com/topameng/CsToLua) - The fastest unity lua binding solution
* [torbensko/Kinect-to-Maya-motion-capture](https://github.com/torbensko/Kinect-to-Maya-motion-capture) - A set of scripts to help you capture the Kinect's motion capture data in Maya
* [torch/DEPRECEATED-torch7-distro](https://github.com/torch/DEPRECEATED-torch7-distro) - Torch7: state-of-the-art machine learning algorithms
* [torch/tds](https://github.com/torch/tds) - Torch C data structures
* [torvalds/linux](https://github.com/torvalds/linux) - Linux kernel source tree
* [toymachine/libredis](https://github.com/toymachine/libredis) - A C based general low-level PHP extension and client library for Redis, focusing on performance, generality and efficient parallel communication with multiple Redis servers. As a bonus, a  Ketama Consistent Hashing implementation is provided as well.
* [tpoechtrager/cctools-port](https://github.com/tpoechtrager/cctools-port) - Apple cctools port for Linux, *BSD and Windows (Cygwin)
* [tpoindex/crobots](https://github.com/tpoindex/crobots) - CROBOTS is a programming game, for programmers (or aspiring programmers.)
* [traildb/traildb](https://github.com/traildb/traildb) - TrailDB is an efficient tool for storing and querying series of events
* [trailofbits/cb-multios](https://github.com/trailofbits/cb-multios) - DARPA Challenges Sets for Linux, Windows, and macOS
* [trailofbits/ctf](https://github.com/trailofbits/ctf) - CTF Field Guide
* [traviscross/mtr](https://github.com/traviscross/mtr) - Official repository for mtr, a network diagnostic tool
* [traviskaufman/MaxCurl](https://github.com/traviskaufman/MaxCurl) - Data retrieval client for MaxMSP
* [trezor/trezor-core](https://github.com/trezor/trezor-core) - :lock: TREZOR Core
* [trezor/trezor-crypto](https://github.com/trezor/trezor-crypto) - :orange_book: Heavily optimized cryptography algorithms for embedded devices.
* [triSYCL/triSYCL](https://github.com/triSYCL/triSYCL) - Modern C++ for accelerators based on SYCL from Khronos Group
* [triaquae/CrazyEye](https://github.com/triaquae/CrazyEye) - OpenSource IT Automation Software
* [trink/hindsight](https://github.com/trink/hindsight) - Hindsight - light weight data processing skeleton
* [tristanheaven/asteroids](https://github.com/tristanheaven/asteroids) - Asteroid taxonomic classification using light curve data
* [troglobit/finit](https://github.com/troglobit/finit) - Fast init for Linux systems. Cookies included
* [troglobit/inadyn](https://github.com/troglobit/inadyn) - Dynamic DNS client with SSL/TLS support
* [tronkko/dirent](https://github.com/tronkko/dirent) - C/C++ library for retrieving information on files and directories
* [troydhanson/kvspool](https://github.com/troydhanson/kvspool) - A library to support streaming data applications
* [troydhanson/tpl](https://github.com/troydhanson/tpl) - tpl - a small binary serialization library for C
* [troydhanson/uthash](https://github.com/troydhanson/uthash) - C macros for hash tables and more
* [tsgates/mbox](https://github.com/tsgates/mbox) - A lightweight sandbox tool for non-root users
* [tsuna/contextswitch](https://github.com/tsuna/contextswitch) - Little micro-benchmark for Linux to test the cost of context switching and system calls
* [tsuraan/Jerasure](https://github.com/tsuraan/Jerasure) - Github repo for Jerasure Library - C Implementation of Reed-Solomon coding
* [tsznxx/wLib](https://github.com/tsznxx/wLib) - Python Modules for High-throughput Sequencing Data Analysis
* [tuanpmt/esp_mqtt](https://github.com/tuanpmt/esp_mqtt) -  MQTT client library for ESP8266 Soc
* [tvheadend/tvheadend](https://github.com/tvheadend/tvheadend) - Tvheadend is a TV streaming server for Linux supporting DVB-S, DVB-S2, DVB-C, DVB-T, ATSC, IPTV,SAT>IP and other formats through the unix pipe as input sources.
* [tvondra/pg_check](https://github.com/tvondra/pg_check) - a tool to verify integrity of PostgreSQL data files
* [twitter/fatcache](https://github.com/twitter/fatcache) - Memcache on SSD
* [twitter/jvmgcprof](https://github.com/twitter/jvmgcprof) - A simple utility for profile allocation and garbage collection activity in the JVM
* [twitter/twemcache](https://github.com/twitter/twemcache) - Twemcache is the Twitter Memcached
* [twitter/twemproxy](https://github.com/twitter/twemproxy) - A fast, light-weight proxy for memcached and redis
* [twogood/dynamite](https://github.com/twogood/dynamite) - PKWARE Data Compression decompressor tool and library
* [tyler/Bogart](https://github.com/tyler/Bogart) - It's like Sinatra... in C.
* [u0u0/Quick-Cocos2dx-Community](https://github.com/u0u0/Quick-Cocos2dx-Community) - Cocos2d-Lua 社区版
* [uTox/uTox](https://github.com/uTox/uTox) - µTox the lightest and fluffiest Tox client
* [ubixum/UXN1212_firmware](https://github.com/ubixum/UXN1212_firmware) - Firmware for the Ubixum UXN1212 USB data acquisition board
* [uci-cbcl/EXTREME](https://github.com/uci-cbcl/EXTREME) - An online EM implementation of the MEME model for fast motif discovery in large ChIP-Seq and DNase-Seq Footprinting data
* [uclouvain/openjpeg](https://github.com/uclouvain/openjpeg) - Official repository of the OpenJPEG project
* [udp/json-parser](https://github.com/udp/json-parser) - Very low footprint JSON parser written in portable ANSI C
* [udp/lacewing](https://github.com/udp/lacewing) - Cross-platform network I/O library for C/C++
* [ufjf-dcc/dsgraph](https://github.com/ufjf-dcc/dsgraph) - DSGraph is an C/C++ library for visualizing data structures.
* [ufo-kit/ufo-core](https://github.com/ufo-kit/ufo-core) - GLib-based framework for GPU-based data processing
* [ufoym/RecursiveBF](https://github.com/ufoym/RecursiveBF) - A lightweight C++ library for recursive bilateral filtering [Yang, Qingxiong. "Recursive bilateral filtering". European Conference on Computer Vision, 2012].
* [ufoym/recursive-bf](https://github.com/ufoym/recursive-bf) - A lightweight C++ library for recursive bilateral filtering [Yang, Qingxiong. "Recursive bilateral filtering". European Conference on Computer Vision, 2012].
* [ultralight-ux/ultralight](https://github.com/ultralight-ux/ultralight) - Ultralight— a lightweight, pure-GPU, HTML UI renderer for C++
* [umitanuki/s3_fdw](https://github.com/umitanuki/s3_fdw) - foreign-data wrapper for Amazon S3
* [umitanuki/tinyint-postgresql](https://github.com/umitanuki/tinyint-postgresql) - A tiny int implementation as a data type of PostgreSQL
* [unbit/spockfs](https://github.com/unbit/spockfs) - SpockFS is an HTTP based network filesystem
* [unbit/uwsgi](https://github.com/unbit/uwsgi) - uWSGI application server container
* [universal-ctags/ctags](https://github.com/universal-ctags/ctags) - A maintained ctags implementation
* [unrealircd/unrealircd](https://github.com/unrealircd/unrealircd) - Official UnrealIRCd repository. Downloads are available from our site
* [uranushiko/Yeelink](https://github.com/uranushiko/Yeelink) - My project used to send data to Yeelink.
* [urbit/archaeology](https://github.com/urbit/archaeology) - An Operating Function
* [urbit/urbit](https://github.com/urbit/urbit) - An operating function
* [urcu/userspace-rcu](https://github.com/urcu/userspace-rcu) - This repo is a mirror of the official lttng-tools git found at git://git.lttng.org/userspace-rcu.git. liburcu is a LGPLv2.1 userspace RCU (read-copy-update) library. This data synchronization library provides read-side access which scales linearly with the number of cores.
* [usrbinnc/netcat-cpi-kernel-module](https://github.com/usrbinnc/netcat-cpi-kernel-module) - Kernel module edition of the Cycles Per Instruction (2014) album.
* [uzbl/uzbl](https://github.com/uzbl/uzbl) - A web browser that adheres to the unix philosophy.
* [v92/libiorouter](https://github.com/v92/libiorouter) - libiorouter is LD_PRELOAD library for caching data and metadata requests from backend directory to local directory transparently to application.
* [valotrading/tick](https://github.com/valotrading/tick) - Tick, a market data tool.
* [valr/cbatticon](https://github.com/valr/cbatticon) - A lightweight and fast battery icon that sits in your system tray
* [vanhauser-thc/thc-hydra](https://github.com/vanhauser-thc/thc-hydra) - hydra
* [varnish/Varnish-Cache](https://github.com/varnish/Varnish-Cache) - Moved. New address: https://github.com/varnishcache/varnish-cache/
* [varnish/hitch](https://github.com/varnish/hitch) - A scalable TLS proxy.
* [varnish/libvmod-cookie](https://github.com/varnish/libvmod-cookie) - A Varnish module for simpler use of the cookie header.
* [varnish/libvmod-curl](https://github.com/varnish/libvmod-curl) - cURL bindings for Varnish through the Varnish Module interface
* [varnishcache/varnish-cache](https://github.com/varnishcache/varnish-cache) - Varnish Cache source code repository
* [vdloo/Beacontalk](https://github.com/vdloo/Beacontalk) - Peer to peer chat-program that sends data over Wi-Fi without associations.
* [vdrolia/speed_hash](https://github.com/vdrolia/speed_hash) - Hash a lot of data as fast as you can
* [veracrypt/VeraCrypt](https://github.com/veracrypt/VeraCrypt) - Disk encryption with strong security based on TrueCrypt
* [verement/cellminer](https://github.com/verement/cellminer) - Bitcoin miner for the Cell Broadband Engine Architecture
* [versatica/OverSIP](https://github.com/versatica/OverSIP) - OverSIP: the SIP framework you dreamed about
* [verse/verse](https://github.com/verse/verse) - Network protocol for real-time sharing between graphical applications
* [verzhak/sfire](https://github.com/verzhak/sfire) - Quantum GIS plugin for mapping of burnt forest areas using Landsat 5 data sets
* [vhmth/Lego-Box](https://github.com/vhmth/Lego-Box) - Write up all the data structures!
* [vi/chaoticfs](https://github.com/vi/chaoticfs) - Encrypting FUSE filesystem with "false bottom" allowing exposing the data only partially
* [vi/fdlinecombine](https://github.com/vi/fdlinecombine) - Read multiple fds and print data to stdout linewise.
* [videolan/vlc](https://github.com/videolan/vlc) - VLC media player - All pull requests are ignored, please follow https://wiki.videolan.org/Sending_Patches_VLC/
* [vifm/vifm](https://github.com/vifm/vifm) - Vifm is a file manager with curses interface, which provides Vi[m]-like environment for managing objects within file systems, extended with some useful ideas from mutt.
* [vijay03/optfs](https://github.com/vijay03/optfs) - The Optimistic File System (OptFS) is a Linux ext4 variant that implements Optimistic Crash Consistency, a new approach to crash consistency in journaling file systems. OptFS improves performance for many workloads, sometimes by an order of magnitude. OptFS provides strong consistency, equivalent to data journaling mode of ext4.
* [vim/vim](https://github.com/vim/vim) - The official Vim repository
* [vimfung/LuaScriptCore](https://github.com/vimfung/LuaScriptCore) - 一款简单易用的多平台Lua桥接器，目前支持在iOS、Mac OS X、Android以及Unity3D中使用，让原生环境与Lua无障碍沟通。
* [vincentbernat/bootstrap.c](https://github.com/vincentbernat/bootstrap.c) - Boilerplate for small C projects (autotools)
* [vincenthz/libjson](https://github.com/vincenthz/libjson) - a JSON parser and printer library in C. easy to integrate with any model.
* [vinniefalco/LuaBridge](https://github.com/vinniefalco/LuaBridge) - A lightweight, dependency-free library for binding Lua to C++
* [virtio-win/kvm-guest-drivers-windows](https://github.com/virtio-win/kvm-guest-drivers-windows) - Windows paravirtualized
* [visit1985/mdp](https://github.com/visit1985/mdp) - A command-line based markdown presentation tool.
* [vivekannan/calc](https://github.com/vivekannan/calc) - Simple command-line based calculator.
* [vivien/i3blocks](https://github.com/vivien/i3blocks) - A flexible scheduler for i3bar
* [vjeux/jspp](https://github.com/vjeux/jspp) - C++ shaped into Javascript
* [vk-com/kphp-kdb](https://github.com/vk-com/kphp-kdb) - VK-KittenPHP/DB/Engine suite
* [vkholodkov/nginx-upload-module](https://github.com/vkholodkov/nginx-upload-module) - A module for nginx web server for handling file uploads using multipart/form-data encoding (RFC 1867).
* [vladimirvivien/go-cshared-examples](https://github.com/vladimirvivien/go-cshared-examples) - Calling Go Functions from Other Languages using C Shared Libraries
* [vlfeat/vlfeat](https://github.com/vlfeat/vlfeat) - An open library of computer vision algorithms
* [vlm/asn1c](https://github.com/vlm/asn1c) - The ASN.1 Compiler
* [vmayoral/bb_mpu9150](https://github.com/vmayoral/bb_mpu9150) - BeagleBone ROS package that publishes the Invensense MPU-9150 data into a Topic.
* [vmayoral/freeDDS](https://github.com/vmayoral/freeDDS) - An open source Data Distribution Service (DDS) for embedded devices implemented for ROS
* [vmg/clar](https://github.com/vmg/clar) - What tests are made of.
* [vmg/crustache](https://github.com/vmg/crustache) - The templating engine which may explode right under your nose
* [vmg/houdini](https://github.com/vmg/houdini) - The Escapist
* [vmg/redcarpet](https://github.com/vmg/redcarpet) - The safe Markdown parser, reloaded.
* [vmg/rinku](https://github.com/vmg/rinku) - Autolinking. Ruby. Yes, that's pretty much it.
* [vmg/sundown](https://github.com/vmg/sundown) - Standards compliant, fast, secure markdown processing library in C
* [vmprof/vmprof-python](https://github.com/vmprof/vmprof-python) - vmprof - a statistical program profiler
* [vmt/udis86](https://github.com/vmt/udis86) - Disassembler Library for x86 and x86-64
* [vndmtrx/libadt](https://github.com/vndmtrx/libadt) - :vertical_traffic_light:libadt - an abstract data types library
* [vonzhou/CSAPP](https://github.com/vonzhou/CSAPP) - CSAPP,《深入理解计算机系统结构》2nd ，阅读与实践！
* [vozlt/nginx-module-sysguard](https://github.com/vozlt/nginx-module-sysguard) - Nginx sysguard module
* [vozlt/nginx-module-vts](https://github.com/vozlt/nginx-module-vts) - Nginx virtual host traffic status module
* [vpereira/pcapreader](https://github.com/vpereira/pcapreader) - saving pcap data on mongodb//tests with and without capped collections
* [vrogier/ocilib](https://github.com/vrogier/ocilib) - OCILIB (C and C++ Drivers for Oracle) - Open source C and C++ library for accessing Oracle databases
* [vsbuffalo/seqqs](https://github.com/vsbuffalo/seqqs) - seqqs is a C program/library for gathering quality statistics from sequencing data
* [vstakhov/libucl](https://github.com/vstakhov/libucl) - Universal configuration library parser
* [vstakhov/rspamd](https://github.com/vstakhov/rspamd) - Rapid spam filtering system.
* [vtudose/Let-s-build-a-compiler](https://github.com/vtudose/Let-s-build-a-compiler) - A C version of the Let's Build a Compiler, by Jack Crenshaw
* [vurtun/gui](https://github.com/vurtun/gui) - A lightweight ANSI C imgui toolkit
* [vurtun/mmx](https://github.com/vurtun/mmx) - single header libraries for C/C++
* [vurtun/zahnrad](https://github.com/vurtun/zahnrad) - A small ANSI C gui toolkit
* [vvv/under.c](https://github.com/vvv/under.c) - DER data decoder/encoder
* [vysheng/tg](https://github.com/vysheng/tg) - telegram-cli
* [wahern/cqueues](https://github.com/wahern/cqueues) - Continuation Queues: Embeddable asynchronous networking, threading, and notification framework for Lua on Unix.
* [wahern/dns](https://github.com/wahern/dns) - dns.c: Single file non-blocking DNS C library without callbacks or external dependencies.
* [wandenberg/nginx-push-stream-module](https://github.com/wandenberg/nginx-push-stream-module) - A pure stream http push technology for your Nginx setup. Comet made easy and really scalable.
* [wangkuiwu/datastructs_and_algorithm](https://github.com/wangkuiwu/datastructs_and_algorithm) - Data struct and algorithm introduction and implementation in C/C++/Java.
* [wankdanker/node-unixodbc-isql-json](https://github.com/wankdanker/node-unixodbc-isql-json) - A hacky solution for querying ODBC data sources (including MS SQL) with nodejs.
* [wargio/r2dec-js](https://github.com/wargio/r2dec-js) - radare2 plugin - converts asm to pseudo-C code.
* [warmcat/libwebsockets](https://github.com/warmcat/libwebsockets) - canonical libwebsockets.org websocket library
* [waruqi/tbox](https://github.com/waruqi/tbox) - A glib-like multi-platform c library
* [wasabiz/xrope](https://github.com/wasabiz/xrope) - rope data structure
* [watmough/jwHash](https://github.com/watmough/jwHash) - Simple hash table implementation for C.
* [wbhart/Cesium3](https://github.com/wbhart/Cesium3) - Fast interpreter with macros, local type inference, LLVM backend.
* [wbhart/comb](https://github.com/wbhart/comb) - Combinators in C
* [wc-duck/dbgtools](https://github.com/wc-duck/dbgtools) - Small collection of debug-related drop-in c/c++-utils
* [wdas/partio](https://github.com/wdas/partio) - C++ (with python bindings) library for easily reading/writing/manipulating common animation particle formats such as PDB, BGEO, PTC.   See the discussion group @ http://groups.google.com/group/partio-discuss
* [wdas/ptex](https://github.com/wdas/ptex) - Per-Face Texture Mapping for Production Rendering
* [wdlindmeier/Interferometer-Watch](https://github.com/wdlindmeier/Interferometer-Watch) - A data visualization to observe the state of LIGO machines
* [webcpp/hi-nginx](https://github.com/webcpp/hi-nginx) - A fast and robust web server and application server for C++,Python,Lua ,Java, PHP7,Javascript and multiple jsr-223 JVM language
* [webglearth/gdaldem_web](https://github.com/webglearth/gdaldem_web) - Utility for encoding elevation data (DEM) for use on the web (with WebGL Earth). Elevation value is encoded into RGB.
* [weechat/weechat](https://github.com/weechat/weechat) - The extensible chat client.
* [welefen/SetCard](https://github.com/welefen/SetCard) - a brain & puzzle game by cocos2d-html5
* [wellsie1116/Darxen](https://github.com/wellsie1116/Darxen) - Downloader, parser, and renderer for NEXRAD data
* [wengkai/ACLLib](https://github.com/wengkai/ACLLib) - ACLLib is a bunch of C functions covers Win32API and provides simpler API to beginners for programming Windows GUI applications. It compiles with MinGW and MS Visual Studio Express
* [wenjun1055/c](https://github.com/wenjun1055/c) - C语言学习代码
* [wernerd/ZRTPCPP](https://github.com/wernerd/ZRTPCPP) - C++ Implementation of ZRTP protocol - GNU ZRTP C++
* [wertarbyte/tiny-gps](https://github.com/wertarbyte/tiny-gps) - read NMEA data from serial GPS receiver (and sonar and optical sensor)  and offer it as I2C slave using ATTiny
* [wesleyd/charade](https://github.com/wesleyd/charade) - Ssh-agent clone for cygwin that proxies to pageant
* [wesleykendall/mpitutorial](https://github.com/wesleykendall/mpitutorial) - MPI programming lessons in C and executable code examples
* [westes/flex](https://github.com/westes/flex) - The Fast Lexical Analyzer - scanner generator for lexing in C and C++
* [wez/lemon-php](https://github.com/wez/lemon-php) - A PHP parser generator, based on the lemon parser generator tool. lemon-php requires a C compiler to build, and this will generate pure-PHP parsers.
* [wezm/open2300](https://github.com/wezm/open2300) - Open2300 is a package of software tools that reads (and writes) data from a Lacrosse WS23xx Weather Stations. This repo is an import of the official SVN repo with some additions.
* [wg/wrk](https://github.com/wg/wrk) - Modern HTTP benchmarking tool
* [wiire/pixiewps](https://github.com/wiire/pixiewps) - An offline WPS bruteforce utility
* [wiiudev/libwiiu](https://github.com/wiiudev/libwiiu) - Build system and examples for running C code on the Wii U
* [wikrsh/hello_fdw](https://github.com/wikrsh/hello_fdw) - Hello world program for PostgreSQL's foreign data wrapper(FDW)
* [willemt/cbuffer](https://github.com/willemt/cbuffer) - A circular buffer written in C using Posix calls to create a contiguously mapped memory space. BSD Licensed.
* [willemt/pearldb](https://github.com/willemt/pearldb) - A Lightweight Durable HTTP Key-Value Pair Database in C
* [willemt/raft](https://github.com/willemt/raft) - C implementation of the Raft Consensus protocol, BSD licensed
* [williame/hellepoll](https://github.com/williame/hellepoll) - A blazingly-fast async HTTP server written in C++
* [wilseypa/odroidNetworking](https://github.com/wilseypa/odroidNetworking) - Data/code/notes relating to our studies with low latency networking and big.LITTLE task assignment on the odroid platform
* [winnukem/racehound](https://github.com/winnukem/racehound) - Data race detector for Linux kernel modules
* [winton/redis_parse](https://github.com/winton/redis_parse) - Reads huge amounts of pipe-delimited data from Redis, filters it, and returns counts by occurence
* [wiredtiger/wiredtiger](https://github.com/wiredtiger/wiredtiger) - WiredTiger's source tree
* [wishstudio/flinux](https://github.com/wishstudio/flinux) - Foreign LINUX - Run unmodified Linux applications inside Windows.
* [wizzard/libtprint](https://github.com/wizzard/libtprint) - TPrint is a simple C library to print ASCII tabular data.
* [wkoszek/cpu60](https://github.com/wkoszek/cpu60) - Example of CPU simulation in software
* [wmutils/core](https://github.com/wmutils/core) - Set of window manipulation tools
* [wolkykim/libasyncd](https://github.com/wolkykim/libasyncd) - Embeddable Event-based Asynchronous Message/HTTP Server library for C/C++
* [wolkykim/qlibc](https://github.com/wolkykim/qlibc) - qLibc is a simple and powerful C library
* [woodrow/cidr-report_analysis](https://github.com/woodrow/cidr-report_analysis) - Data processing & analysis tools to replicate the CIDR Report and study Internet route aggregation.
* [wouterverweirder/AIR-Sudden-Motion-Sensor-Extension](https://github.com/wouterverweirder/AIR-Sudden-Motion-Sensor-Extension) - Native Extension for Adobe AIR, exposing the sudden motion sensor data of mac portables in your AIR application
* [wren-lang/wren](https://github.com/wren-lang/wren) - The Wren Programming Language
* [wtangiit/awesim](https://github.com/wtangiit/awesim) - event-driven simulator for data aware distributed workflow system
* [wujunze/nginx-http-echo-module](https://github.com/wujunze/nginx-http-echo-module) - A simple Nginx echo module
* [wukezhan/air](https://github.com/wukezhan/air) - a high performance, lightweight framework for php5 & php7 written in c
* [x2on/libssh2-for-iOS](https://github.com/x2on/libssh2-for-iOS) - A script for compiling libssh2 for iOS Devices (iPhone, iPad, iPod Touch). The example app can connect to an server with SSH and execute commands.
* [x86-64/frozen](https://github.com/x86-64/frozen) - Data management and processing library
* [x893/CMSIS-DAP](https://github.com/x893/CMSIS-DAP) - STM32 port for CMSIS-DAP with additional serial (CDC) support
* [xaberus/nih](https://github.com/xaberus/nih) - libnih, the library interactive data dumper will be based upon
* [xaionaro/clsync](https://github.com/xaionaro/clsync) - file live sync daemon based on inotify/kqueue/bsm (Linux, FreeBSD), written in GNU C
* [xant/XML-TinyXML](https://github.com/xant/XML-TinyXML) - minimal perl-xs module to handle XML data
* [xant/libhl](https://github.com/xant/libhl) - Simple and fast C library implementing a thread-safe API to manage hash-tables, linked lists, lock-free ring buffers and queues
* [xavier-chen/simplep2p](https://github.com/xavier-chen/simplep2p) - Test NAT Traversal after using pjnath to see if we can send data to peer
* [xbmc/android](https://github.com/xbmc/android) - OBSOLETE Android port. Now merged into mainline!
* [xcir/libvmod-parsereq](https://github.com/xcir/libvmod-parsereq) - parsing post,get,cookie data
* [xelatihy/yocto-gl](https://github.com/xelatihy/yocto-gl) - A collection of C/C++ single-file libraries for building physically-based graphics applications
* [xelerance/Openswan](https://github.com/xelerance/Openswan) - Openswan
* [xemul/criu](https://github.com/xemul/criu) - Checkpoint/Restore tool
* [xeniaqian94/Reliable-Data-Transfer-3.0-Protocol-Networking](https://github.com/xeniaqian94/Reliable-Data-Transfer-3.0-Protocol-Networking) - Project of COMP 3234, Computer and Communication Networks
* [xerpi/libsicksaxis](https://github.com/xerpi/libsicksaxis) - SickSaxis is a C library that lets you connect a Sixaxis or a DualShock3 to the Wii and read its data. It also lets you turn on and off the controller LEDs, enable or disable the rumble and get and set the controllers' bluetooth MAC address.
* [xiao70/X70FSD](https://github.com/xiao70/X70FSD) - Windows file system filter drivers(minifilter) to encrypt, compress, or otherwise modify file-based data require some of the most complex kernel software developed for Windows.
* [xiehuc/pidgin-lwqq](https://github.com/xiehuc/pidgin-lwqq) - a pidgin plugin based on lwqq, a excellent safe useful library for webqq protocol
* [xiph/flac](https://github.com/xiph/flac) - Free Lossless Audio Codec
* [xiph/opus](https://github.com/xiph/opus) - Modern audio compression for the internet.
* [xiph/rnnoise](https://github.com/xiph/rnnoise) - Recurrent neural network for audio noise reduction
* [xjdrew/lua-zset](https://github.com/xjdrew/lua-zset) - lua data structure same as redis sorted set
* [xlar54/Commodore-Pi](https://github.com/xlar54/Commodore-Pi) - A native Commodore 64 emulator and operating system for the Raspberry Pi
* [xnko/libapi](https://github.com/xnko/libapi) - libapi is a cross platform high performance io library written in c. It provides ability to write event driven servers and applications with continous code
* [xobs/ax2xx-code](https://github.com/xobs/ax2xx-code) - Some code for the AX211 or AX215 8051-based CPU
* [xoreaxeaxeax/movfuscator](https://github.com/xoreaxeaxeax/movfuscator) - The single instruction C compiler
* [xorg62/tty-clock](https://github.com/xorg62/tty-clock) - Clock using lib ncurses
* [xroche/coffeecatch](https://github.com/xroche/coffeecatch) - CoffeeCatch, a tiny native POSIX signal catcher (especially useful for JNI code on Android/Dalvik)
* [xsawyerx/xs-fun](https://github.com/xsawyerx/xs-fun) - XS is fun: a simple and easy tutorial on writing Perl XS
* [xstevens/decoderbufs](https://github.com/xstevens/decoderbufs) - A PostgreSQL logical decoder output plugin to deliver data as Protocol Buffers
* [xtaci/libkcp](https://github.com/xtaci/libkcp) - FEC enhanced KCP session library for iOS/Android in C++
* [xtacocorex/CHIP_IO](https://github.com/xtacocorex/CHIP_IO) - A CHIP IO library for Python: IO+PWM+SPWM+ADC+Utilities
* [xurenlu/ngx_mem_backend_module](https://github.com/xurenlu/ngx_mem_backend_module) - simple nginx module to fetch data from memcached and echo data;
* [xwang149/Dsim](https://github.com/xwang149/Dsim) - Data transfer simulator
* [xxorde/librekinect](https://github.com/xxorde/librekinect) - Depth data from a kinect sensor! Small and fast kernel driver. Also for embedded devices like the raspberry pi!
* [xyjax/sdd2json](https://github.com/xyjax/sdd2json) - EVE static data dump to JSON exporter
* [y123456yz/Reading-and-comprehense-linux-Kernel-network-protocol-stack](https://github.com/y123456yz/Reading-and-comprehense-linux-Kernel-network-protocol-stack) - linux内核网络协议栈源码阅读分析注释--带详尽中文分析注释以及相关流程分析调用注释，对理解分析内核协议栈源码很有帮助
* [y123456yz/reading-code-of-nginx-1.9.2](https://github.com/y123456yz/reading-code-of-nginx-1.9.2) - nginx-1.9.2源码通读分析注释，带详尽函数中文分析注释以及相关函数流程调用注释，最全面的nginx源码阅读分析中文注释，更新完毕
* [yaderbh/dstruct](https://github.com/yaderbh/dstruct) - An object oriented implementation of data structures for PHP
* [yaml/libyaml](https://github.com/yaml/libyaml) - Canonical source repository for LibYAML
* [yaouser/C](https://github.com/yaouser/C) - linux下的C语言及关于kernel的介绍
* [yaoweibin/nginx_tcp_proxy_module](https://github.com/yaoweibin/nginx_tcp_proxy_module) - add the feature of tcp proxy with nginx, with health check and status monitor
* [yarikoptic/NiPy-OLD](https://github.com/yarikoptic/NiPy-OLD) - Analysis of structural and functional neuroimaging data in Python (yet not stabilized -- fork on your risk)
* [yarrick/iodine](https://github.com/yarrick/iodine) - Official git repo for iodine dns tunnel
* [yarrick/pingfs](https://github.com/yarrick/pingfs) - Stores your data in ICMP ping packets
* [yasm/yasm](https://github.com/yasm/yasm) - Yasm Assembler mainline development tree
* [yellows8/ctr-httpwn](https://github.com/yellows8/ctr-httpwn) - 3DS HTTP-sysmodule exploit for bypassing required sysupdates.
* [yixuan/fdaplus](https://github.com/yixuan/fdaplus) - Enhancement of the 'fda' package for functional data analysis
* [yl790/algorithms-and-data-structures](https://github.com/yl790/algorithms-and-data-structures) - for future reference
* [yomoncada/C-Language](https://github.com/yomoncada/C-Language) - First steps of my C Language programing.
* [yongboy/c_socket.io_server](https://github.com/yongboy/c_socket.io_server) - The socket.io Linux C server
* [yosefk/checkedthreads](https://github.com/yosefk/checkedthreads) - checkedthreads: no race condition goes unnoticed! Simple API, automatic load balancing, Valgrind-based checking
* [yotamr/traces](https://github.com/yotamr/traces) - API tracing framework for Linux C/C++ applications
* [youngsterxyf/Data-Structures-and-Algorithms](https://github.com/youngsterxyf/Data-Structures-and-Algorithms) - simple implementation of some data structures and algorithms
* [yourtion/30dayMakeOS](https://github.com/yourtion/30dayMakeOS) - 《30天自制操作系统》源码中文版。自己制作一个操作系统（OSASK）的过程
* [yourtion/LearningMasteringAlgorithms-C](https://github.com/yourtion/LearningMasteringAlgorithms-C) - Mastering Algorithms with C 《算法精解：C语言描述》源码及Xcode工程、Linux工程
* [youzan/zan](https://github.com/youzan/zan) - 高效稳定、安全易用、线上实时验证的全异步高性能网络库，通过PHP扩展方式使用。
* [yrutschle/sslh](https://github.com/yrutschle/sslh) - Applicative Protocol Multiplexer (e.g. share SSH and HTTPS on the same port)
* [yunnian/php-nsq](https://github.com/yunnian/php-nsq) - a php nsq client write by c extension,the fastest  nsq client
* [yurial/tread](https://github.com/yurial/tread) - read file, exit at no data when timed out
* [yuriks/SHView](https://github.com/yuriks/SHView) - Spherical Harmonics data viewer
* [yusugomori/DeepLearning](https://github.com/yusugomori/DeepLearning) - Deep Learning (Python, C/C++, Java, Scala, Go)
* [yuya-takeyama/hashtable_dump](https://github.com/yuya-takeyama/hashtable_dump) - A Zend Extension to dump HashTable data structure on Zend Engine.
* [yuyuyu101/C-Buffered-tree](https://github.com/yuyuyu101/C-Buffered-tree) - A buffered-tree implemented in dictionary type and more
* [yyuu/pyenv](https://github.com/yyuu/pyenv) - Simple Python version management
* [z3APA3A/3proxy](https://github.com/z3APA3A/3proxy) - 3proxy - tiny free proxy server
* [zammitjames/dataparksearch](https://github.com/zammitjames/dataparksearch) - Full featured web search engine
* [zaphire/Monocle-Engine](https://github.com/zaphire/Monocle-Engine) - Open source game engine for lush 2D. Inspired by Aquaria, FlashPunk and Unity.
* [zardus/preeny](https://github.com/zardus/preeny) - Some helpful preload libraries for pwning stuff.
* [zarya/esp8266_i2c_driver](https://github.com/zarya/esp8266_i2c_driver) - ESP8266 I2C Driver
* [zdevito/ATen](https://github.com/zdevito/ATen) - ATen: A TENsor library for C++11
* [zebrafishlabs/nginx-statsd](https://github.com/zebrafishlabs/nginx-statsd) - An nginx module for sending stats to statsd.
* [zedshaw/learn-c-the-hard-way-lectures](https://github.com/zedshaw/learn-c-the-hard-way-lectures) - All of the code from Learn C The Hard Way, each project, plus the presentation slides used in the videos.
* [zedshaw/liblcthw](https://github.com/zedshaw/liblcthw) - The library you create when you are done with Learn C The Hard Way
* [zeevt/csnappy](https://github.com/zeevt/csnappy) - Google snappy in C for Linux Kernel
* [zenovich/runkit](https://github.com/zenovich/runkit) - Runkit that works!
* [zeromq/czmq](https://github.com/zeromq/czmq) - High-level C binding for ØMQ
* [zeromq/rbzmq](https://github.com/zeromq/rbzmq) - Ruby binding for 0MQ
* [zeromq/zyre](https://github.com/zeromq/zyre) - Zyre - an open-source framework for proximity-based peer-to-peer applications
* [zfogg/ascii-chat](https://github.com/zfogg/ascii-chat) - ASCII video chat.
* [zfsonlinux/spl](https://github.com/zfsonlinux/spl) - Solaris Porting Layer
* [zfsonlinux/zfs](https://github.com/zfsonlinux/zfs) - Native ZFS for Linux
* [zfsrogue/zfs-crypto](https://github.com/zfsrogue/zfs-crypto) - ZFS On Linux with crypto patches
* [zhaojh329/libumqtt](https://github.com/zhaojh329/libumqtt) - A Lightweight and fully asynchronous MQTT 3.1.1 client C library based on libubox for Embedded Linux. Support QoS 0, 1 and 2. Support ssl.
* [zhaojh329/libuwsc](https://github.com/zhaojh329/libuwsc) - A Lightweight and fully asynchronous WebSocket client C library based on libubox for Embedded Linux.
* [zhemao/libds](https://github.com/zhemao/libds) - Simple, memory-safe data-structures in C.
* [zhengshuxin/acl](https://github.com/zhengshuxin/acl) - One advanced C/C++ library for Linux/Mac/FreeBSD/Solaris(x86)/Windows/Android/IOS
* [zhicheng/db](https://github.com/zhicheng/db) - A New DBM in Pure C
* [zlib-ng/zlib-ng](https://github.com/zlib-ng/zlib-ng) - zlib replacement with optimizations for "next generation" systems.
* [zmap/zmap](https://github.com/zmap/zmap) - ZMap Internet Scanner
* [zmartzone/mod_auth_openidc](https://github.com/zmartzone/mod_auth_openidc) -  OpenID Connect Relying Party and OAuth 2.0 Resource Server for Apache HTTP Server 2.x
* [znort987/blockparser](https://github.com/znort987/blockparser) - Simple C++ bitcoin blockchain parser
* [zpl-c/zpl](https://github.com/zpl-c/zpl) - 📐 Your C99 Powerkit
* [zsaleeba/picoc](https://github.com/zsaleeba/picoc) - A very small C interpreter
* [zserge/partcl](https://github.com/zserge/partcl) - ParTcl - a micro Tcl implementation
* [zserge/webview](https://github.com/zserge/webview) - Tiny cross-platform webview library for C/C++/Golang. Uses WebKit (Gtk/Cocoa) and MSHTML (Windows)
* [zsh-users/zsh](https://github.com/zsh-users/zsh) - Mirror of the Z shell source code repository.
* [zsummer/breeze](https://github.com/zsummer/breeze) - 一个C++的轻量级的分布式服务器引擎, 架构思想为一切皆service.
* [zsummer/zsummerX](https://github.com/zsummer/zsummerX) - zsummerX is a cross-platform C++ high performance lightweight network library. via IOCP/EPOLL/SELECT.
* [zupet/LuaTinker](https://github.com/zupet/LuaTinker) - LUA to C++ Binding Library
* [zwdzwd/biscuit](https://github.com/zwdzwd/biscuit) - a little tool for bisulfite data


# Fin #

[484]: https://www.codeproject.com/Articles/6154/Writing-Efficient-C-and-C-Code-Optimization
[483]: https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.p
[482]: https://www.chiark.greenend.org.uk/~sgtatham/mp/
[481]: http://www.greenend.org.uk/rjk/tech/inline.html
[480]: http://snaipe.me/c/c-smart-pointers/
[479]: https://graphics.stanford.edu/~seander/bithacks.html
[478]: http://danluu.com/malloc-tutorial/
[477]: http://250bpm.com/blog:56
[476]: http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html
[475]: https://proprogramming.org/some-unknown-features-or-tricks-in-c-language/
[474]: https://hintjens.gitbooks.io/scalable-c/content/index.html
[473]: https://computing.llnl.gov/tutorials/mpi/
[472]: https://computing.llnl.gov/tutorials/openMP/
[471]: https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG
[470]: https://nullprogram.com/blog/2017/03/30
[469]: https://nullprogram.com/blog/2015/02/17
[468]: https://jvns.ca/blog/2014/12/14/fun-with-threads/
[467]: http://mpitutorial.com/
[466]: http://blog.noctua-software.com/c-tricks.html
[465]: https://blogs.oracle.com/linux/8-gdb-tricks-you-should-know-v2
[464]: http://blog.pkh.me/p/20-templating-in-c.html
[462]: https://computing.llnl.gov/tutorials/pthreads/
[461]: https://web.archive.org/web/20170620131430/https://www.tedunangst.com/flak/post/memcpy-vs-memmove
[460]: https://www.recurse.com/blog/5-learning-c-with-gdb
[459]: https://gist.github.com/eatonphil/21b3d6569f24ad164365

[457]: http://nethack4.org/blog/building-c.html
[456]: http://nullprogram.com/blog/2017/08/20/
[455]: https://pdos.csail.mit.edu/6.828/2017/readings/pointers.pdf
[454]: http://nullprogram.com/blog/2017/09/21/
[453]: http://www.etalabs.net/compare_libcs.html
[452]: http://c-faq.com/
[451]: https://locklessinc.com/benchmarks_allocator.shtml

[440]: https://github.com/alanxz/rabbitmq-c
[439]: https://github.com/dertuxmalwieder/libvldmail
[438]: https://github.com/nfc-tools/libnfc
[437]: https://github.com/cloudwu/pbc
[436]: http://sourceware.org/binutils/docs/bfd/
[435]: https://gnu.org/software/gss/
[434]: https://github.com/swenson/sort
[433]: https://github.com/antirez/linenoise
[432]: https://github.com/recp/tm
[431]: http://kitsune-dsu.com/
[430]: http://www.colm.net/open-source/ragel/
[429]: http://libcello.org/
[428]: https://github.com/jeremyevans/ape_tag_libs/tree/master/c
[427]: https://criu.org/Main_Page
[426]: https://github.com/sinemetu1/twitc
[425]: https://www.gnu.org/software/gnulib/
[423]: https://github.com/obgm/libcoap
[422]: https://gnu.org/software/freeipmi/index.html
[421]: https://github.com/commonmark/cmark/blob/master/COPYING
[420]: https://github.com/commonmark/cmark
[419]: https://en.wikipedia.org/wiki/Knuth's_Algorithm_X
[418]: https://github.com/blynn/dlx
[417]: https://github.com/simplegeo/libgeohash
[416]: https://github.com/google/gumbo-parser
[415]: https://glade.gnome.org/
[414]: https://www.gnu.org/software/gperf/
[413]: https://brechtsanders.github.io/xlsxio/

[412]: https://github.com/docopt/docopt.c
[411]: https://github.com/cofyc/argparse
[410]: https://github.com/jibsen/parg

[409]: https://github.com/google/cpu_features
[408]: https://github.com/libimobiledevice/libimobiledevice
[407]: https://libusb.info/

[406]: http://www.dyncall.org/
[405]: https://gnu.org/software/libffcall/
[404]: https://github.com/atgreen/libffi

[403]: http://libcox.symisc.net/
[402]: https://github.com/dmw/caffeine
[401]: http://savannah.nongnu.org/projects/attr/

[400]: http://libevent.org/
[399]: http://software.schmorp.de/pkg/libev.html
[398]: http://facebook.github.io/libphenom/index.html
[397]: http://libuv.org

[396]: https://github.com/openvenues/libpostal
[395]: http://libtrading.org/
[394]: https://tulipindicators.org/

[393]: http://www.throwtheswitch.org/cexception
[392]: https://github.com/esneider/debug
[391]: http://hardysimpson.github.io/zlog/
[390]: https://github.com/gpakosz/whereami

[389]: https://lodev.org/lodepng/
[388]: https://github.com/mozilla/mozjpeg
[387]: http://www.vips.ecs.soton.ac.uk/index.php?title=VIPS
[386]: https://wiki.gnome.org/action/show/Projects/LibRsvg?action=show&redirect=LibRsvg
[385]: http://www.libpng.org/
[384]: https://libjpeg-turbo.virtualgl.org/
[383]: https://pngquant.org/lib/
[382]: https://github.com/prideout/heman
[381]: https://sourceforge.net/projects/giflib/
[380]: https://github.com/libgd/libgd

[379]: https://github.com/codeplea/tinyexpr
[378]: https://github.com/riolet/WAFer
[377]: http://www.pell.portland.or.us/~orc/Code/discount/
[376]: https://github.com/jgm/cmark
[375]: https://github.com/hoedown/hoedown
[374]: https://github.com/nsf/termbox
[373]: https://gnu.org/software/ncurses/
[372]: https://github.com/sabotage-linux/netbsd-curses
[371]: https://github.com/doches/progressbar
[370]: https://github.com/zeromq/zproto


[364]: https://kore.io/
[363]: http://www.koanlogic.com/klone/
[362]: http://facil.io/
[361]: https://dasoftver.bitbucket.io/cloudgizer

[360]: http://re2c.org/index.html
[359]: https://github.com/orangeduck/mpc
[358]: https://github.com/abiggerhammer/hammer
[357]: https://www.gnu.org/software/bison/
[356]: https://github.com/westes/flex

[355]: https://github.com/evolutional/utest
[354]: http://www.throwtheswitch.org/unity
[353]: https://wiki.haskell.org/Introduction_to_QuickCheck2
[352]: https://github.com/silentbicycle/theft
[351]: https://nemequ.github.io/munit
[350]: https://github.com/codeplea/minctest
[349]: https://github.com/silentbicycle/greatest
[348]: http://cunit.sourceforge.net/
[347]: https://github.com/bvdberg/ctest
[346]: https://criterion.readthedocs.io/en/master
[345]: https://cmocka.org/
[344]: http://www.throwtheswitch.org/cmock
[343]: https://github.com/vmg/clar
[342]: https://github.com/yhfudev/cpp-ci-unit-test.git
[341]: https://libcheck.github.io/check
[340]: http://users.jyu.fi/~sapekiis/cheat

[339]: https://github.com/Juniper/libxo
[338]: https://github.com/vstakhov/libucl
[337]: https://github.com/0intro/libelf
[336]: https://github.com/martinh/libconfuse
[335]: https://github.com/mongodb/libbson
[334]: https://www.pyyaml.org/wiki/LibYAML
[333]: http://xmlsoft.org/
[332]: http://expat.sourceforge.net/
[331]: https://madmurphy.github.io/libconfini/html/index.html
[330]: https://github.com/ndevilla/iniparser
[329]: https://github.com/benhoyt/inih
[328]: https://lloyd.github.io/yajl/
[327]: https://github.com/netmail-open/wjelement/
[326]: https://github.com/sheredom/json.h
[325]: https://zserge.com/jsmn.html
[324]: https://github.com/NeonMercury/jfes
[323]: http://www.digip.org/jansson/
[322]: https://github.com/rgamble/libcsv

[321]: https://github.com/JuliaLang/utf8proc
[320]: https://github.com/sheredom/utf8.h
[319]: http://tartarus.org/martin/PorterStemmer/
[318]: https://github.com/wooorm/stmr.c
[317]: https://github.com/antirez/sds
[316]: https://boyerjohn.github.io/rapidstring/index.html
[315]: https://github.com/josephg/librope
[314]: https://gnu.org/software/libiconv/
[313]: https://gnu.org/software/libunistring/
[312]: https://en.wikipedia.org/wiki/Levenshtein_distance
[311]: https://github.com/wooorm/levenshtein.c
[310]: http://site.icu-project.org/
[309]: http://mike.steinert.ca/bstring/

[308]: https://uclibc-ng.org/
[307]: http://pdclib.e43.eu/
[306]: https://www.musl-libc.org/
[305]: https://www.gnu.org/software/libc/
[304]: https://www.fefe.de/dietlibc/
[303]: https://en.wikipedia.org/wiki/Capability-based_security
[302]: https://github.com/NuxiNL/cloudlibc
[301]: https://github.com/aosp-mirror/platform_bionic

[300]: https://github.com/RandyGaul/tinyheaders
[299]: https://github.com/nothings/stb
[298]: https://github.com/DanielGibson/Snippets/
[297]: https://github.com/prideout/par
[296]: https://github.com/vurtun/mmx
[295]: http://www.fefe.de/djb/
[294]: https://github.com/clibs/clib/wiki/Packages
[293]: https://github.com/clibs/clib
[292]: http://ccodearchive.net/

[291]: https://en.wikipedia.org/wiki/External_Data_Representation
[290]: https://github.com/troydhanson/tpl
[289]: https://github.com/protobuf-c/protobuf-c
[288]: http://opic.rocks/
[287]: https://github.com/ludocode/mpack
[286]: http://avro.apache.org/docs/current/api/c/index.html#_introduction_to_avro_c
[285]: https://google.github.io/flatbuffers/
[284]: https://github.com/dvidelabs/flatcc
[283]: https://msgpack.org/
[282]: https://github.com/camgunz/cmp
[281]: https://github.com/jmckaskill/c-capnproto
[280]: https://github.com/liteserver/binn

[279]: https://github.com/laurikari/tre/
[278]: https://github.com/cesanta/slre
[277]: http://www.pcre.org/
[276]: https://github.com/kkos/oniguruma
[275]: https://github.com/k-takata/Onigmo

[274]: https://bitbucket.org/MDukhan/yeppp
[273]: http://www.libtom.net/TomsFastMath/
[272]: http://slepc.upv.es/
[271]: https://github.com/cvxgrp/scs
[270]: http://www.mcs.anl.gov/petsc/
[269]: http://pari.math.u-bordeaux.fr/
[268]: http://www.libtom.net/LibTomPoly/
[267]: http://www.libtom.net/LibTomMath/
[266]: http://www.netlib.org/lapack/lapacke.html
[265]: https://sourceforge.net/projects/kissfft/
[264]: https://www.gnu.org/software/gsl/
[263]: https://gnu.org/software/mpria/
[262]: http://mpfr.loria.fr/index.html
[261]: http://www.multiprecision.org/index.php?prog=mpc&page=home
[260]: https://gmplib.org/
[259]: https://gnu.org/software/glpk/
[258]: http://flintlib.org/
[257]: http://www.fftw.org/
[256]: https://github.com/adis300/fft-c
[255]: http://www.feynarts.de/cuba/
[254]: https://scientificc.github.io/cmathl/
[253]: https://github.com/clMathLibraries/clBLAS
[252]: http://math-atlas.sourceforge.net/
[251]: https://github.com/fredrik-johansson/arb
[250]: http://apophenia.info

[249]: https://github.com/zeromq/zyre
[248]: https://tatsuhiro-t.github.io/wslay/
[247]: https://github.com/silentbicycle/socket99
[246]: https://gnu.org/software/osip/
[245]: https://nanomsg.github.io/nng/
[244]: https://github.com/nanomsg/nanomsg
[243]: https://cesanta.com
[242]: https://lwan.ws
[241]: https://github.com/JonnyWhatshisface/libwebsock
[240]: https://github.com/LibVNC/libvncserver
[239]: https://risoflora.github.io/libsagui/
[238]: http://sourceforge.net/projects/libquickmail/
[237]: https://www.coralbits.com/libonion/
[236]: https://gnu.org/software/libmicrohttpd/
[235]: https://gnu.org/software/libidn/
[234]: http://www.hughes.com.au/products/libhttpd/
[233]: http://www.etpan.org
[232]: https://curl.haxx.se/libcurl/
[231]: http://www.nlnetlabs.nl/projects/ldns/index.html
[230]: https://github.com/joyent/http-parser
[229]: https://www.gnu.org/software/adns/
[228]: https://github.com/it4e/CHL
[227]: http://lionet.info/asn1c/compiler.html

[226]: http://paulbatchelor.github.io/proj/soundpipe.html
[225]: https://github.com/lieff/minimp3
[224]: http://libsound.io
[223]: http://www.mega-nerd.com/libsndfile/
[222]: https://mpv.io
[221]: https://gstreamer.freedesktop.org/
[220]: https://www.ffmpeg.org/
[219]: https://github.com/aubio/aubio

[218]: https://github.com/minad/tlsf
[217]: http://www.gii.upv.es/tlsf/
[216]: https://talloc.samba.org/talloc/doc/html/index.html
[215]: https://github.com/rampantpixels/rpmalloc
[214]: https://locklessinc.com/
[213]: http://jemalloc.net
[212]: https://www.hboehm.info/gc/

[211]: http://xforms-toolkit.org/
[210]: http://www.tcl.tk/
[209]: https://sourceforge.net/projects/tinyfiledialogs/
[208]: https://github.com/vurtun/nuklear
[207]: http://webserver2.tecgraf.puc-rio.br/iup/
[206]: https://www.gtk.org/

[205]: https://spdx.org/licenses/MPL-1.1.html
[204]: http://www.sgi.com/tech/opengl/?/license.html
[203]: https://www.opengl.org/
[202]: https://github.com/memononen/nanovg
[201]: https://github.com/ands/lightmapper
[200]: https://gnu.org/software/libxmi/
[199]: https://github.com/saitoha/libsixel
[198]: https://github.com/cacalabs/libcaca
[197]: http://ebassi.github.io/graphene/
[196]: http://cairographics.org/

[195]: https://github.com/ferreiradaselva/uastar
[194]: https://clover.moe/spearmint
[193]: http://www.libsigil.com/
[192]: https://github.com/grimfang4/sdl-gpu
[191]: https://www.libsdl.org/
[190]: https://www.libretro.com/
[189]: https://github.com/libretro/RetroArch
[188]: https://www.raylib.com
[187]: https://github.com/id-Software/Quake-2
[186]: https://github.com/id-Software/Quake
[185]: http://orx-project.org
[184]: https://github.com/ferreiradaselva/mathc
[183]: https://xiph.org/ao/
[182]: https://github.com/Kazade/kazmath
[181]: https://ioquake3.org
[180]: https://www.glfw.org/
[179]: http://freeglut.sourceforge.net
[178]: https://github.com/shlomif/fc-solve
[177]: https://github.com/anholt/libepoxy
[176]: https://icculus.org/twilight/darkplaces/
[175]: https://www.sfml-dev.org/index.php
[174]: https://www.sfml-dev.org/download/csfml/
[173]: https://github.com/orangeduck/Corange
[172]: http://chipmunk-physics.net
[171]: https://github.com/recp/cglm
[170]: https://liballeg.org

[169]: http://cyan4973.github.io/xxHash
[168]: https://github.com/leo-yuriev/t1ha
[167]: https://github.com/centaurean/spookyhash
[166]: https://github.com/google/highwayhash
[165]: https://github.com/lemire/clhash

[164]: https://github.com/waruqi/tbox
[163]: http://wolkykim.github.io/qlibc
[162]: http://www.mission-base.com/peter/source/
[161]: http://www.koanlogic.com/libu/
[160]: https://github.com/keybuk/libnih
[159]: http://libcork.readthedocs.io/en/0.14.0/
[158]: http://attractivechaos.github.io/klib/#About
[157]: https://www.enlightenment.org
[156]: http://www.eso.org/sci/software/cpl/
[155]: https://fragglet.github.io/c-algorithms
[154]: http://apr.apache.org/
[65]: https://github.com/parallella/pal

[120]: http://www.doxygen.nl/
[119]: https://hplgit.github.io/doconce/doc/web/index.html
[118]: http://www.gedanken.org.uk/software/cxref/

[107]: https://github.com/swenson/vector.h
[106]: http://troydhanson.github.io/uthash/
[105]: https://github.com/gpakosz/PackedArray
[104]: https://github.com/nbulischeck/list.h
[103]: https://faragon.github.io/libsrt.html
[102]: https://github.com/theck01/offbrand_lib
[101]: https://github.com/P-p-H-d/mlib
[100]: http://liblfds.org/
[99]: https://igraph.org/
[98]: https://github.com/recp/ds
[97]: http://adtinfo.org/libavl.html/index.html
[96]: https://github.com/jtsiomb/kdtree
[95]: https://github.com/srdja/Collections-C
[58]: https://github.com/xant/libhl

[94]: http://whitedb.org/
[93]: https://unqlite.org/
[92]: https://www.sqlite.org/
[91]: https://github.com/spotify/sparkey
[90]: http://sophia.systems
[89]: https://redis.io/
[88]: https://www.postgresql.org/
[87]: https://symas.com/lightning-memory-mapped-database/
[86]: http://mongoc.org/
[85]: https://github.com/redis/hiredis
[84]: https://github.com/groonga/groonga
[83]: http://www.oracle.com/us/products/database/berkeley-db

[82]: https://github.com/trezor/trezor-crypto
[81]: http://www.saphir2.com/sphlib/
[80]: https://github.com/awslabs/s2n
[79]: http://maciejczyzewski.me/retter/
[78]: https://github.com/miracl/MIRACL
[77]: https://tls.mbed.org/
[76]: https://www.libtom.net
[75]: https://download.libsodium.org/doc
[74]: https://openquantumsafe.org/
[73]: https://www.openssl.org/source/license.html
[72]: https://www.openssl.org/
[71]: https://gnupg.org/related_software/libgcrypt
[70]: http://www.gnutls.org/
[69]: https://gnu.org/software/gsasl/

[68]: https://tinycthread.github.io/
[67]: https://en.wikipedia.org/wiki/POSIX_Threads
[66]: https://gnu.org/software/pth/
[64]: https://www.open-mpi.org/
[63]: https://www.openmp.org/
[62]: http://tuxfan.github.io/ocl-mla/
[61]: https://github.com/matze/oclkit
[60]: http://libmill.org/
[59]: http://liburcu.org/
[57]: http://libdill.org/
[56]: https://github.com/sharow/libconcurrent
[55]: http://www.shlomifish.org/rwlock/
[54]: http://concurrencykit.org
[53]: https://github.com/yosefk/checkedthreads
[52]: http://repo.hu/projects/cchan/

[51]: http://facebook.github.io/zstd/
[50]: https://github.com/Dead2/zlib-ng
[49]: https://github.com/libarchive/libarchive
[48]: http://zlib.net
[47]: https://github.com/kuba--/zip
[46]: https://github.com/powturbo/TurboRLE
[45]: https://github.com/powturbo/TurboPFor
[44]: https://github.com/quixdb/squash
[43]: https://github.com/antirez/smaz
[42]: https://github.com/lemire/simdcomp
[41]: http://ed-von-schleck.github.io/shoco
[40]: https://github.com/vasi/pixz
[39]: http://www.oberhumer.com/opensource/lzo/
[38]: http://lz4.github.io/lz4/
[37]: https://github.com/inikep/lizard
[36]: http://www.bzip.org/
[35]: https://github.com/adamierymenko/huffandpuff
[34]: https://github.com/gildor2/fast_zlib
[33]: https://github.com/atomicobject/heatshrink
[32]: https://github.com/centaurean/density
[31]: https://github.com/Cyan4973/FiniteStateEntropy
[30]: http://roaringbitmap.org/
[29]: https://github.com/RoaringBitmap/CRoaring
[28]: http://lzip.nongnu.org/lzip.html
[27]: http://lzip.nongnu.org/clzip.html
[26]: https://github.com/google/brotli
[25]: http://blosc.org/pages/blosc-in-depth


[10]: https://github.com/jppbsi/LibDEEP/wiki
[9]: https://github.com/attractivechaos/kann
[8]: https://codeplea.com/genann
[7]: http://leenissen.dk/fann/wp/
[6]: https://github.com/100/Cranium
[5]: http://libccv.org

[AFL-2.1]: https://spdx.org/licenses/AFL-2.1.html
[AGPL-3.0-only]: https://spdx.org/licenses/AGPL-3.0-only.html
[AGPL-3.0-or-later]: https://spdx.org/licenses/AGPL-3.0-or-later.html
[Apache-2.0]: https://spdx.org/licenses/Apache-2.0.html
[BSD-1-Clause]: https://spdx.org/licenses/BSD-1-Clause.html
[BSD-2-Clause]: https://spdx.org/licenses/BSD-2-Clause.html
[BSD-3-Clause]: https://spdx.org/licenses/BSD-3-Clause.html
[BSD-4-Clause]: https://spdx.org/licenses/BSD-4-Clause.html
[CC0-1.0]: https://spdx.org/licenses/CC0-1.0.html
[curl]: https://spdx.org/licenses/curl.html
[GPL-2.0-only]: https://spdx.org/licenses/GPL-2.0-only.html
[GPL-2.0-or-later]: https://spdx.org/licenses/GPL-2.0-or-later.html
[GPL-3.0-only]: https://spdx.org/licenses/GPL-3.0-only.html
[GPL-3.0-or-later]: https://spdx.org/licenses/GPL-3.0-or-later.html
[ICU]: https://spdx.org/licenses/ICU.html
[ISC]: https://spdx.org/licenses/ISC.html
[LGPL-2.0-or-later]: https://spdx.org/licenses/LGPL-2.0-or-later.html
[LGPL-2.1-only]: https://spdx.org/licenses/LGPL-2.1-only.html
[LGPL-2.1-or-later]: https://spdx.org/licenses/LGPL-2.1-or-later.html
[LGPL-3.0-only]: https://spdx.org/licenses/LGPL-3.0-only.html
[LGPL-3.0-or-later]: https://spdx.org/licenses/LGPL-3.0-or-later.html
[Libpng]: https://spdx.org/licenses/Libpng.html
[MIT]: https://spdx.org/licenses/MIT.html
[MPL-2.0]: https://spdx.org/licenses/MPL-2.0.html
[NCSA]: https://spdx.org/licenses/NCSA.html
[OLDAP-2.8]: https://spdx.org/licenses/OLDAP-2.8.html
[PostgreSQL]: https://spdx.org/licenses/PostgreSQL.html
[TCL]: https://spdx.org/licenses/TCL.html
[Unlicense]: https://spdx.org/licenses/Unlicense.html
[WTFPL]: https://spdx.org/licenses/WTFPL.html
[X11]: https://spdx.org/licenses/X11.html
[Zlib]: https://spdx.org/licenses/Zlib.html
