# Fork
## int fork()
### Description
Creates a new process by duplicating the calling process. The new process is called the child and the calling process the parent.

### Arguments
The fork function has no arguments.

# Stat
### Description
Returns information about a file.

### Arguments
- const char* path: path of the file
- struct stat* buf: buffer for file information

# kill
### Description
Sends any signal to any process.

### Arguments
- pid_t pid: process id
- int sig: signal id

# chmod
### Description
Changes the files mode.

### Arguments
- const char* pathname: filepath
- mode_t mode: new mode

# waitpid
### Description
Suspends execution of the calling process until a child has changed state. It waits only for terminated children except if options arguments has been modified.

### Arguments
- pid_t pid: process id of child process
- int* status: status of child process
- int options: behavior of the function

# Fails
- fork: no memory left
- exec: an I/O error occures
- unlink: not enough memory is available
- read: fd is not valid descriptor
- mount: component of path not searchable
- chmod: pathname is too long
- kill: invalid signal

# Trap
A trap is a instruction to get access to the kernel space, to be able to use system calls.