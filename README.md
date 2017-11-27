# Posit-HDL-Arithmetic
"Universal number (Unum) Posit HDL Arithmetic Architecture Generator"

A parameterized Verilog HDL for Unum Posit number system arithmetic is
under progress. At present, it includes the basic arithmetic of Floating-Point 
to Posit conversion, Posit to Floating-Point conversion, Posit addition/subtraction, 
Posit Multiplication. Addition module can also be used for subtraction, just by
negating second operand.

At current, round-to-zero rounding method is incorporated in these units, which
will be updated for other rounding methods soon.

The Infinity and Not-A-Number (NaN) cases are handled as per the exact Posit
standards as provided in its original paper. According to it, Posit format does
not support/include NaN, which is considered as Infinity in current HDL
generation.

Posit standards are followed from the developer's paper which can be find at
http://www.johngustafson.net/pdfs/BeatingFloatingPoint.pdf
