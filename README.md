# Digital IC Design Homework

## DIC HW2-BoothAlgorithm

### Introduction
- Booth algorithm is a multiplication operation that multiplies two numbers in two's complement notation. The detail algorithm is described as below:
  1. Assume that the multiplicand m is x-bit and multiplier r is .y-bit. Initialize a register P for the final result, and the length is x+y+l bits. The initial value of P is 0(x bits)_r(y bits)_0(l bit).
  2. The rightmost 2 bits used for the selection of different executions.

    | LSB | Execution                            |
    | --- | ---                                  |
    |  00 | No execution                         |
    |  01 | Add *m* to the left part of P        |
    |  10 | Subtract *m* from the left part of P |
    |  11 | No execution                         |
    
    > \* all of the overflow can be ignored during the execution

  3. **Arithmetically** shift 1 bit on P.
  4. Repeat the step ii.. and iii.. for 7 times.
  5. The final answer is obtained by dropping the LSB from P.



## AUTHORS
[Yu-Tong Shen](https://github.com/yutongshen/)
