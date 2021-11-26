# I. Introduction
> Initialized: 2021-11-25. Last edited: 2021-11-25.

## 1.1 How to Build an LFS System

### Host system
- LFS systems need to be built using an already installed Linux distributions.
    - The host will be the starting point of the project by providing necessary programs:
        - compiler, linker, shell to build the new system.
    - Select the "development" option during the distribution installation to be able to access these tools.

### Chapters

#### Chapter 2
- Describes how to create new Linux native partitions and the file system. New Linux systems are compiled and installed on there.


#### Chapter 3 
- Explains which packages and patches are needed to be downloaded to build an LFS system and how to store them on the new file system.

#### Chapter 4 
- Discusses the setup of an appropriate working environment.
    - This chapter necessitates particular attention because it explains several important issues needs to be aware of before proceeding onwards in the book.

#### Chapter 5 
- Explains the installation of the initial tool chain:
    - binutils, gcc, glibc
- using cross-compilation techniques to isolate the new tools from the host system.

#### Chapter 6
- Shows you how to cross-compile basic utilities using the recently built cross-toolchain.

#### Chapter 7
- Enter into a "chroot" environment that uses the previously built tools to build the additional tools needed to build and test the final system.
- This effort to isolate the new system from the host distribution may seem excessive. A full technical explanation as to why this is done is provided in (Toolchain Technical Notes)[https://www.linuxfromscratch.org/lfs/view/stable/partintro/toolchaintechnotes.html].

#### Chapter 8
- The full LFS system is *built* in this chapter.
- Another advantage provided by a chroot environment is the ability for the user to continue using the host system whilst LFS is being built.
    - You can use your computer as normal while waiting for package compilations to complete.

#### Chapter 9
- To finish *installation*, basic system configuration is set up.

#### Chapter 10
- The kernel and boot-loader are set up.

#### Chapter 11
- Contains information on continuing the LFS experience beyond this book.
- After the steps in this book have been implemented, the computer will be ready to reboot into the new LFS system.

This is the process simply put. Detailed information for each step is discussed in the following chapters and respective package descriptions.

Seemingly complicated items will be clarified. **Everything will fall into place as you embark on the LFS adventure.**
