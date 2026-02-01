# Linux core concept
* **The Kernel** : This is the heart and core of Linux os . it is that part who interact with Hardware . it decide who gets memory , how much cpu time get a
                task gets and handle the hardware.
* **User space** : This is where everything lives . They are not allowed to touch hardware directl , they have to ask the kernel for permission.

* **Init/systemd** : This is very first process that starts when you turn on the computer . it is resposible for getting everything else up and running.

# How process created and managed
* Linux user two step program method to start a new program.
* creation : fork and exec
- **Fork** : A process that make copy of itself . The original is the parent and the copy is the child.
- **exec** : the child process , it replace its new program 
* **Management**
-The Kernel acts as a referee. Since a CPU can only do one thing at a time (very quickly), the Kernel performs Context Switching. it gives Process A
a few milliseconds of time, pauses it, gives Process B a few milliseconds, and rotates. This happens so fast it feels like everything is running at
once.

# systemd
* The Master controller - parent of all process (PID 1)
* Parrallel Booting - start services at same time , making you computer faster
* Service Healing - restart the crash server

# The Lifecycle : process states
* **Running** : The process is either using the CPU or waiting in line to use it. it is active and healthy
*  **sleeping** : interruptible(S) and unintruptible (d)
*  **stopped** : you havemanualy pause the process and waiting for start
*  **Zombie** : This is a process that has finished its job, but its "parent" hasn't acknowledged it yet.
  
# Daily use commands
* ls -l
* ls -a
* grep
* chmod/chown
* df -h
* tail -f
    -  

















