# ROC24_4sz_ISA_encoding and ROC24_4sz_binary_sort
Have done binary encoding of the ISA for four data types and four data sizes  
The encoding PDF is by op-code category and the sort PDF is by binary op-code  
Have no intention of doing a full implementation, e.g. many op-codes are reserved  
The vast majority of the 40 and 48-bit instructions are unallocated,  
and could be used for additional 24 and 32-bit instructions  
## The set of data types under consideration are
  Unsigned binary  
  Two's complement binary  
  Sign and magnitude with negative zero code used as missing or invalid  
  IEEE 754 floating-point with denorms flushed to zero  
  Modified 754 with gradual underflow and gradual overflow,  
    supporting both exact and inexact values,  
    with inexact values rounded to nearest half odd  
# ROC24_ISA_detail and ROC24_opcode_sort  
PDF files with binary encoding of the op-codes  
The instructions are of either 24 or 32 bits  
Each instruction and its formats are listed  
There is op-code space reserved for 40 and 48-bit instructions  
The 24 and 32-bit formats are 80% full, and it is likely the  
48-bit instruction category will support multiple instruction lengths  
Some details still in flux.  Supported/non-supported op-codes TBD  
# ROC32_8  
Specification for implementation of a 32-bit RISC architecture  
There are 32 registers of 32 bits  
Memory has a 32-bit byte address  
Instructions can be 24, 32, 40 or 48 bits long  
Current status is: specification  
# ROCnn_mm  
The ROCnn_32_231122 files have details on the nn = 36, 42 & 48-bit word size variants  
Which offers data sizes of 36, 42 and 48-bits and their submultiples  
And has a separate byte addressable instruction memory  
And uses an external DRAM memory of 256-bit chunks  
# TROCnn_mm  
The TROC variant has register type fields for each register in the register file  
Which simplifies the ISA by implying operation type from operand types  
