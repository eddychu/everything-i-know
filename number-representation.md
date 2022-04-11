All complex digital system that thrives in today's world have a rather humble beginning. All information, being an ebook you read, the conversation you had with your whatsapp friends, your favorite youtube videos, all of them are encoded in 0 and 1s.

To understand the details of how information is represented in digital world, we need to start with simple things.

## Integer number

We humans use a numeral system based on 10 digits (0 - 9), which is called the decimal numeral system. Unlike us, residents in digital world only speaks only 1s and 0s, so naturally they represent things in binary forms.

To facilitate communication from Planet Earth to Planet Digital we need a mechanism to translate decimal froms to binary forms.

A 10-based decimal number has the general form of  d<sub>n</sub>d<sub>n-1</sub>d<sub>n-2</sub>...d<sub>0</sub> = d<sub>n</sub> * 10<sup>n</sup> + d<sub>n-1</sub> * 10<sup>n-1</sup> + d<sub>n-2</sub> * 10<sup>n-2</sup> + ... + d<sub>0</sub> * 10<sup>0</sup>

Following the this pattern, a binary number can also be represented in similar form:

b<sub>n</sub>b<sub>n-1</sub>b<sub>n-2</sub>...b<sub>0</sub> =b<sub>n</sub> * 2<sup>n</sup> +  b<sub>n-1</sub> * 2<sup>n-1</sup> + b<sub>n-2</sub> * 2<sup>n-2</sup>...b<sub>0</sub> * 2<sup>0</sup>

```
1984 -> 11111000000
```
## Sign and Unsigned

the aforementioned scheme can only be used to encode positive numbers. 

In order to encode a negative number, the solution is to treat the first bit of a binary number as sign bit. if the sign bit is set (meaning it is set as 1), then the binary number represents a negative number, otherwise, it is positive.

in the signed encoding scheme, the general form of a binary number is:

b<sub>n</sub>b<sub>n-1</sub>b<sub>n-2</sub>...b<sub>0</sub> =-b<sub>n</sub> * 2<sup>n</sup> + b<sub>n-1</sub> * 2<sup>n-1</sup> + b<sub>n-2</sub> * 2<sup>n-2</sup>...b<sub>0</sub> * 2<sup>0</sup>

```
11111000000 ->  
```
signed encoding is called 2's complete.

notice that the same binary number can mean two different numbers depending on signed or unsigned encoding.

the computer need other context information to decide if a certain 0s and 1s pattern should be decoded as signed or unsigned number. But we are getting ahead of ourselves.

## Float number

The practice we adopted for float number encoding is rather odd.

it has the general form V = (-1)<sup>s</sup> * M * 2<sup>E</sup>

Like the signed encoding we introduced for integer numbers, it has a signed bit to determine if the number is negative or positive.

there are two most common formats for floating point number,single pricision (32 bits) and double precision (64 bits).

to do: finish float number examples.

