# ROC32_8  
Specification for implementation of a 32-bit RISC architecture  
There are 32 registers of 32 bits  
Memory has a 32-bit byte address  
Instructions can be 24, 32, 40 or 48 bits long  
Current status is: specification  
  
The ROCnn_32_231122.docx file has details on the nn = 36, 42 and 48-bit word size variants  
Which offers data sizes of 36, 42 and 48-bits and their submultiples  
And has a separate byte addressable instruction memory  
And uses an external DRAM memory of 256-bit chunks  
  
The TROC variant has register type fields for each register in the register file  
Which simplifies the ISA by implying operation type from operand types  
