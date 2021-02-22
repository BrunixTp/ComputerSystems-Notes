# Binary Representation of Numbers

## 1 Numeration Systems and the Representation of Integers

### 1.1 Numeration Systems 

Natural numbers can be represented in any positional numeration system. We normaly use a system that bases on the 10th base (10 diferent digits). Computers are binary machines, because they work using two digits (0 and 1), these digits are known as *bits*, from the english expression *b*inary dig*it*.

In order to understand what the base in each represented number means, we need to remember what the order of each digit means.

The *order* of a digit is given by the position the digit is placed on the number.

#### Example: 
**1532.64 (base 10)**
    Digit 4 - order -2
    Digit 6 - order -1
    Digit 2 - order 0
    Digit 3 - order +1
    Digit 5 - order +2
    Digit 1 - order +3

The *base* used determines the number of digits that can be used: for example, base 10 uses 10 digits (0 to 9), base 2 uses 2 digits (0 and 1), base 5 uses 5 digits (0 to 4), base 16 uses 16 digits (0 to 9 and (either) A to F or a to f).

### 1.2 Conversion between bases

The *conversion* of a number written in the *base b to the decimal base* is done by multiplying each digit by the base b to the power of the digit's order, and the sum of these values.

The *conversion* of a number in the *decimal base to a base b* is done via the **sucessive division of the integer part** and then the **sucessive multiplication of the fractionary part**