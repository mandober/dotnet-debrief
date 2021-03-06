# Numeric Types

https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/integral-types-table


- Integrals (integers)
  - Unsigned
  - Signed
- Floating points
  - Single precision (base 2)
  - Double precision (base 2)
  - Quadruple precision (base 10)


## Debrief: Numbers
- `int` and `long` are first-class types favored by CPU and C#'s Runtime
- `float` and `double` also have good support (CPU and registers)
- `decimal` is about 10x slower then `float`
- `decimal` is also a floating type, but with base 10 exponent.
- suffixes are case insensitive.
- Integrals can also be assigned using hex notation with `0x` prefix.
- Binary notation with `0b` prefix (since C# 7)
- Digits of precision: 7 float, 15-16 double, 28-29 decimal.

> Use `System.Numerics.BigInteger` class to represent an arbitrarily large signed integer.



## Numeric types

| Cs Type | System. | Suf | Size | Range                | Precision |
|---------|--------:|-----|-----:|----------------------|-----------|
| sbyte   |   SByte |     |    8 | -2^7  to  2^7–1      |           |
| short   |   Int16 |     |   16 | –2^15 to 2^15–1      |           |
| int     |   Int32 |     |   32 | –2^31 to 2^31–1      |           |
| long    |   Int64 | L   |   64 | –2^63 to 2^63–1      |           |
| byte    |    Byte |     |    8 | 0 to 2^8–1           |           |
| ushort  |  UInt16 |     |   16 | 0 to 2^16–1          |           |
| uint    |  UInt32 | U   |   32 | 0 to 2^32–1          |           |
| ulong   |  UInt64 | UL  |   64 | 0 to 2^64–1          |           |
| float   |  Single | F   |   32 | ±  ~10^–45 to 10^38  | 7         |
| double  |  Double | D   |   64 | ± ~10^–324 to 10^308 | 15-16     |
| decimal | Decimal | M   |  128 | ±  ~10^–28 to 10^28  | 28-29     |

e.g. `System.Int32 == int`



## Integrals types

| Cs Type | Framework     | Suf | Size |      Range      |
|---------|---------------|-----|-----:|:---------------:|
| byte    | System.Byte   |     |    8 |   0 to 2^8–1    |
| sbyte   | System.SByte  |     |    8 |  -2^7 to 2^7–1  |
| ushort  | System.UInt16 |     |   16 |   0 to 2^16–1   |
| short   | System.Int16  |     |   16 | –2^15 to 2^15–1 |
| uint    | System.UInt32 | U   |   32 |   0 to 2^32–1   |
| int     | System.Int32  |     |   32 | –2^31 to 2^31–1 |
| ulong   | System.UInt64 | UL  |   64 |   0 to 2^64–1   |
| long    | System.Int64  | L   |   64 | –2^63 to 2^63–1 |


There are 4 signed integer types that can be used depending on how large a number you need the variable to hold.

Integers can also be assigned using hexadecimal notation, `0x` prefix
As of C# 7.0, there is a binary notation as well, prefixed with `0b`.

Version 7.0 of C# also added a digit separator (_) to improve readability of long numbers. This digit separator can appear anywhere within the number, as well as at the beginning of the number as of C# 7.2.


## Floating-Point Types

The floating-point types can store real numbers with different levels of precision. Literal (constant) floating-point numbers are always kept as doubles, so in order to assign such a number to a float variable, an F character needs to be appended to convert the number to the float type. The same applies to the M character for decimals.

The precisions of floating-point types refers to the total number of digits that the types can hold.

For example, when attempting to assign more than 7 digits to a float, the least significant ones will get rounded off.

```cs
myFloat = 12345.6789F; // rounded to 12345.68
Floating-point numbers can be assigned using either decimal or
exponential notation, as in the following example.
myDouble = 3e2; // 3*10^2 = 300
```


## Numeric Literals

Integral literals can also use hexadecimal notation:
`long y = 0x7F`

From C#7, underscore is allowed as (ignored) separator:
`int mil = 1_000_000`

From C#7, binary notation:
`var b = 0b1010_1011`

Real literals can also use exponential notation:
`double mil = 1E06`


## Numeric inference

The compiler infers a numeric literal to be a double or an integral:
- `double`: if it contains a decimal point or the exponential symbol (E)
- otherwise, the type is the first type in this list, that can fit the
  literal's value,: `int`, `uint`, `long`, `ulong`.

## Numeric suffixes

- suffixes are case insensitive
- suffixes `U` and `L` are rarely necessary, because the uint, long and ulong
  can nearly always be either inferred or implicitly converted from int:
  long i = 5 (implicit lossless conversion)
- `D` suffix is technically redundant, in that all literals with a decimal
  point are inferred to be double.
- `F` and `M` suffixes should always be applied when specifying a float or
  a decimal. Without the F suffix, this would not compile, because 4.5 would
  be inferred as double, which has no implicit conversion to float:
      float f = 4.5F;
  The same principle is true for a decimal literal:
      decimal d = -1.23M; // Will not compile without the M suffix.


## Numeric Conversions

Conversions are implicit if the destination type can represent every possible value of the source type. Otherwise, an explicit conversion is required.

**between integrals**
- implicit: smaller to bigger
- explicit: bigger to smaller

    int x = 12345;      // 32-bit integer
    long y = x;         // Implicit conversion to 64-bit integer
    short z = (short)x; // Explicit conversion to 16-bit integer

**between floats**
- implicit: `float` to `double`
- explicit: `double` to `float`

**between floating-points and integrals**
- implicit: all integral types to all floating-point types
    int i = 1;
    float f = i;
- explicit: all floating-point types to all integral types
    int i2 = (int)f;






















