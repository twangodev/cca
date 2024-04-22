# Number Systems

## Base 10: Decimal

Only 10 digits exist in the system: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9

Used commonly in math, is the default representation of numbers in Java

## Base 2: Binary

Only uses two digits, 0 and 1

### Storing Binary in Java

To store binary in Java, the `0b` header is used to indicate binary

```java
int x = 0b100110;
```

### Recursively Converting Decimal to Binary

```java
int decimalToBinary(int decimal) {
	if (decimal == 0) return 0;
  return decimalToBinary(decimal / 2) * 10 + decimal % 2;
}
```

#### Base 2 Storage Units

##### Bit

The state of a single bit of memory, whether its `0` or `1`.

##### Byte

8 bits

##### Kilobyte (KB)

1,024 Bytes

##### Megabyte (MB)

1,024 KB

##### Gigabyte (GB)

1,024 MB

## Base 8: Octal

Only 8 digits within the system: 0, 1, 2, 3, 4, 5, 6, 7

### Storing Octal in Java

To store octal in Java, the `0` header is used

```java
int x = 0384;
```

### Converting Decimal to Octal

Similar to [Recursively Converting Decimal to Binary](#recursively-converting-decimal-to-binary), we use the 8 digits instead of 2

```java
int decimalToOctal(int decimal) {
	if (decimal == 0) return 0;
	return decimalToOctal(decimal / 8) * 10 + decimal % 8;
}
```

## Base 16: Hexadecimal

Only 16 digits in the system: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

!!! tip
    Hexadecimal uses characters A-F to represents 10-15, respectively


### Storing Hexadecimal in Java

To store hexadecimal in Java, the `0x` header is used

```java
int x = 0x4CB3;
```

### Converting Decimal to Hexadecimal

```java
String getHexString(int decimal) { // Map hex string to 
	switch (decimal) {
		case 10: return "A";
		case 11: return "B";
		case 12: return "C";
		case 13: return "D";
		case 14: return "E";
		case 15: return "F";
	}
	return Integer.toString(decimal);
}

String decimalToHex(int decimal) {
	if (decimal == 0) return ""; // Will result in empty string if decimal = 0
	return decimalToHex(decimal / 16) + getHexString(decimal % 16);
}
```