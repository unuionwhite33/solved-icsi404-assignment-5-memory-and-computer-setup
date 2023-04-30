Download Link: https://assignmentchef.com/product/solved-icsi404-assignment-5-memory-and-computer-setup
<br>
Part 1

Now that we have an ALU, we need to add some memory to build the next portion of our computer.

Build a class called “memory”. Unlike the ALU, the rippleAdder and the multiplier, the memory needs to have state (members). It should have the following method calls:

public longword read(longword address) public void write(longword address, longword value)

You must hard code the amount of memory our computer will have – 1024 bytes. The storage must be constructed from our existing bit class.

You must provide a test file (memory_test.java) that implements void runTests() and call it from your main, along with your existing tests. As with the other tests, these tests must be independent of each other and there must be reasonable coverage. You cannot reasonably test all of the billions of possible combinations, but you can test a few representative samples.

Part 2

With memory and an ALU, we can start working on building a functional CPU.

Start by creating a class: computer.

Add a bit to indicate if the computer is halted or not. This should default to NOT running (for now).

Create a void run() method that runs in a while loop until the halted bit indicates that the computer should not run anymore. Within this loop, four methods needs to be called: void fetch(), void decode(), void execute(), void store(), in that order.

Add a memory member (private) to your computer.

There are no tests that we can reasonably run on your computer yet.