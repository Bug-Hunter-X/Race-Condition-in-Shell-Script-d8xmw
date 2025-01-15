This repository contains a shell script demonstrating a race condition bug and its solution.

The `bug.sh` script showcases the race condition: multiple processes attempt to increment a counter stored in a file concurrently.  This can lead to incorrect results because of the asynchronous access and potential data loss.

The `bugSolution.sh` demonstrates a solution using file locking to synchronize access to the shared resource, ensuring that only one process can modify the counter at a time.