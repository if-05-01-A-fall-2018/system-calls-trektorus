# Fork
## int fork()
### Description
Creates a new process by duplicating the calling process. The new process is called the child and the calling process the parent.

### Arguments
The fork function has no arguments.

# Stat
### Description
Returns the meta data of a specified file by the path argument and stores it into the buf.

### Arguments
- const char* path: path of the file
- struct stat* buf: buffer for the file information

# kill
### Description
Sends a signal specified by the argument sig to the process with the specified process id pid.

### Arguments
- pid_t pid: process id
- int sig: signal id

# chmod
### Description
Lets you change the file access values like read-access, write-access etc.

### Arguments
- const char* pathname: filepath
- mode_t mode: new access values

# waitpid
### Description
Suspends execution of the calling process until a child has changed state. It only waits for terminated children except if the options arguments has been modified.

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