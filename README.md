# Linux From Scratch
> Initialized: 2021-11-25. Last edited: 2021-11-25.

- Version 11.0. Published September 1st, 2021.
- Online: <https://www.linuxfromscratch.org/lfs/view/stable/>
- My personal notes.

## Preface

### Foreword
- When the hands in deck fail to meet needs, it's best to pull a new one out from scratch. 
- Custom-built Linux systems allow not only serve to meet user-specific system needs but also learning opportunities for many.
- The Linux From Scratch book is the opus magnum of this project. It merely serves to guide the reader to construct a system of their very own.

### Audience
- This knowledge exists to teach how Linux systems work and how operating systems and computers function in general in its completeness.
- It is useful for system administrators.
- LFS enables the creation of very compact Linux systems.
- Education is the most powerful reason to be involved in this project.
    - Understanding in producing a straightforward base Linux system.

### LFS Target Architectures

#### CPUs
- AMD/Intel x86 (32-bit) and x86_64 (64-bit) CPUs.
    - Although, instructions in this book are also known to work, using some modifications, with Power PC and ARM CPUs.
#### Building
- An existing Linux System is needed to build an LFS system.
    - Note that a 32-bit project can be installed and used as the host system on 64-bit AMD/Intel hardware.
- There is little advantage to building 64-bit systems over 32-bit systems. On the same hardware:
    - 64-bit builds are only marginally faster.
    - 32-bit builds are only a quarter smaller.
- The default 64-bit build that results from LFS is considered a "pure" 64-bit system: it only supports 64-bit executables.
    - "multi-lib" systems require compiling many applications twice, once for a 32-bit system and again for a 64-bit system.
    - LFS/BLFS editors maintain a [fork](https://www.linuxfromscratch.org/~thomas/multilib/index.html) multilib for of LFS, but it is an advanced topic.
#### Usage
- As a LAMP server or firewall, 32-bit CPU build may be largely sufficient.
- Several packages in BLFS (Beyond Linux From Scratch) need more than 4GB of RAM.
    - If you plan to use LFS as a desktop, authors recommend building on a 64-bit system.

### Prerequisites
- Existing knowledge of Unix system administration for resolving problems and correctly executing commands listed.
    - using the command line shell, 
    - copying/moving files/directories, 
    - listing directory and file contents,
    - changing current directory,
    - Reasonable knowledge using and installing Linux software.
- Basic questions will be ignored in forums.
- Before building an LFS system (and going through this book), read the following:
    - [Software-Building-HOWTO](http://www.tldp.org/HOWTO/Software-Building-HOWTO.html)
        - comprehensive guide to building and installing "generic" Unix software packages under Linux
        - good summary of basic techniques for building and installing software
    - [Beginner's Guide to Installing from Source](https://www.linuxfromscratch.org/lfs/view/stable/prologue/prerequisites.html)
        - good summary of basic skills needed to build software from source code

### Standards