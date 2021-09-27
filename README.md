# maxsat-solver
MaxSAT solver that implements the Novelty++ algorithm.

## Compilation

Ensure that OpenJDK 14 is installed. for example, in Ubuntu: 'apt install -y openjdk-14-jdk-headless'.

javac MaxSATSolver.java

## Runtime

java -Xmx8g MaxSATSolver NumberOfThreads TimeLimitInMinutes < file

The '-Xmx8g' flag tells the runtime to allocate up to 8 GB of heap memory. This is necessary for large problem sizes, since the default heap memory size may not be enough.

For example:
java -Xmx8g MaxSATSolver 4 15 < max-sat-problem-200-3-869-1.txt

This will run with 4 worker threads, and will timeout after 15 minutes. The problem will be read from the file 'max-sat-problem-200-3-869-1.txt'.


