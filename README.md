# LLCGX
Loop-Less Code Generator for small even size matrices multiplication (for AMD processor  systems) 


This work was performed at the Argonne National Laboratory, Argonne, Illinois
from year 2009 to year 2011.

The ANL invention number: IN-11-081, title "Loop-Less Code
Generator for Well Defined Computational Tasks."  
Inventor: Jesse Y. Wang.  And DOE Case number: S-127,593.

The Loopless Assembly Code Generator will produce loop-less assembly code to do small matrice multiplications,
where the matrices are stored in double precision row-wise (such as in C-programming language), for AMD-64 
processor based computer systems only,  using gcc compiler.
  

Define the sizes of double precision matrices A, B, and C,  where A x B = C, and
A is of dimension M by K, and matrix B is of the dimension K by N, then
matrix C is of the dimension M by N, where M, K, N are small even integers, say, less than 10.

The output is an assembly listing file, named dgemmrMbNbK in D: (flash driver).  It is stored as a text file.
User can change the file type to .s file, then use gcc compiler to execute the assembly programs.
