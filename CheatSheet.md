# Cheat Sheet C++

## Primitive Types

### Bits
1 byte == 8 bits  
1 kilobyte == 1,000 bytes == 8,000 bits  
1 megabyte == 1,000,000 bytes == 8,000,000 bits

| | Little Endian | Big Endian |
| -- | -- | -- |
| LSB | Right to Left | Left to Right |
| MSB | Left to Right | Right to Left |

**Binary Translator**

| $\frac{Position}{Decimal}$ | 8 | 7 | 6 | 5 | 4 | 3 | 2 | 1 | 0 |
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | ``` 1 ``` |
| 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | ``` 1 ``` | 0 |
| 4 | 0 | 0 | 0 | 0 | 0 | 0 | ``` 1 ``` | 0 | 0 |
| 8 | 0 | 0 | 0 | 0 | 0 | ``` 1 ``` | 0 | 0 | 0 |
| 16 | 0 | 0 | 0 | 0 | ``` 1 ``` | 0 | 0 | 0 | 0 |
| 32 | 0 | 0 | 0 | ``` 1 ``` | 0 | 0 | 0 | 0 | 0 |
| 64 | 0 | 0 | ``` 1 ``` | 0 | 0 | 0 | 0 | 0 | 0 |
| 128 | 0 | ``` 1 ``` | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 256 | ``` 1 ``` | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
 
#### Bitwise Operators

| Operator | Name | Usage | Result | Math |
| -------- | ---- | ----- | ------ | ---- |
| >> | shift right | ``` 0b0100 >> 1 ``` | ``` 0b0010 ``` | $4/2=2$ |
| << | shift left | ``` 0b0100 << 1 ``` | ``` 0b1000 ``` | $4*2=8$ |
| ``` & ``` | AND | ``` 0b0010 & 0b1010 ``` | TODO | TODO |
| ``` \| ```| OR  | ``` 0b0010 \| 0b1010 ``` | TODO | TODO |
| ``` ^ ``` | XOR | ``` 0b0010 ^ 0b1010 ``` | TODO | TODO |
| ``` ~ ``` | NOT | ``` 0b0010 ~ 0b1010 ``` | TODO | TODO |

**AND** (``` & ```) Truth Table
| A | B | Result | Logical |
| -- | -- | -- | -- |
| 0 | 0 | 0 | ``` false && false == false ``` |
| 0 | 1 | 0 | ``` false && true == false ``` |
| 1 | 0 | 0 | ``` true && true == false ``` |
| 1 | 1 | 1 | ``` true && true == true ``` |

**OR** (``` | ```) Truth Table
| A | B | Result | Logical |
| -- | -- | -- | -- |
| 0 | 0 | 0 | ``` false \|\| false == false ``` |
| 0 | 1 | 1 | ``` false \|\| true == true ``` |
| 1 | 0 | 1 | ``` true \|\| false == true ``` |
| 1 | 1 | 1 | ``` true \|\| true == true ``` |

**XOR** (``` ^ ```) Truth Table
| A | B | Result |
| -- | -- | -- |
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

**NOT** (``` ~ ```) Truth Table
| A | Result | Logical |
| -- | -- | -- |
| 0 | 1 | ``` !0 == 1 ``` |
| 1 | 0 | ``` !1 == 0 ``` |

### Fundamental Data Types

| Type | Format | Size | Range |
| -- | -- | -- | -- |
| char | signed | 8 bits | -128 , 127 |
|  | unsigned | 8 bits | 0 , 255 |
| short | signed | 16 bits | $\pm$ 3.27 $\times10^4$ |
|  | unsigned | 16 bits | 0 , 6.55 $\times10^4$ |
| int | signed | 32 bits | $\pm$ 2.14 $\times10^9$ |
|  | unsigned | 32 bits | 0 , 4.29 $\times10^9$ |
| long | signed | 64 bits | $\pm$ 9.22 $\times10^{18}$ |
|  | unsigned | 64 bits | 0 , 1.84 $\times10^{19}$ |
| size_t | unsigned |  >= 16 bits | *compiler dependent* |

## Arrays

## Strings

## Linked Lists

## Stacks and Queues

## Binary Trees

## Heaps

## Searching

## Hash Tables

## Sorting

## Binary Search Trees

## Recursion

## Dynamic Programming

## Greedy Algorithms and Invariants

## Graphs

## Parallel Computing

## Other
