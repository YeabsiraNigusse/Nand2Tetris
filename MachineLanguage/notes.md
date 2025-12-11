## Machine language

- If you wish to understand a system, or build one, start by studying the function that the system is supposed to serve.
- After all, executing programs written in machine language efficiently is the ultimate function of any general-purpose computer.
- Machine language is the most profound interface in the computer enterprise—the fine line where hardware meets software
- In fact, just as we say that the machine language is designed to control a particular hardware platform
- A machine language can be viewed as an agreed-upon formalism designed to manipulate a memory using a processor and a set of registers.
- In the early days of computer systems, computers were programmed manually: 

        When proto-programmers wanted to issue the instruction “set R1 to the value of R1 + R2”, they pushed up and down mechanical switches that stored a binary code like 1010110001000001 in the computer’s instruction memory. And if the program was a hundred instructions long, they had to go through this ordeal a hundred times. Of course debugging such programs was a perfect nightmare. 
        
        This led programmers to invent and use symbolic codes as a convenient way for documenting and debugging programs on paper, before entering them into the computer. 
        
        For example, the symbolic format `add R2,R1` could be chosen for representing the semantics `set R1 to the value of R1 + R2` and the binary instruction 1010110001000001.
- The design of the Hack computer, which will be presented in the next chapter, follows a widely used hardware paradigm known as the von Neumann architecture

        @7
        D=A   // puts 7 into D

        @100
        M=1   // means RAM[100] = 1

        D=3
        D=D+1   // now D=4

        @21
        D=A      // D = 21
        @10
        M=D      // RAM[10] = 21

        @10
        D=M      // D = RAM[10] = 21