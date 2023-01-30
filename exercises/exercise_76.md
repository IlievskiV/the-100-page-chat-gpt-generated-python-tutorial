# Exercise 76
Please write a program to compress and decompress the string "hello world!hello world!hello world!hello world!".

## Code
```python
import zlib

t = zlib.compress(b'hello world!hello world!hello world!hello world!')
print(t)
print(zlib.decompress(t))
```

## ChatGPT Explanation
The code is using the `zlib` library to perform data compression and decompression. The `zlib` library provides in-memory compression and decompression functions, including the compress and decompress functions.

In the code, the string `"hello world!hello world!hello world!hello world!"` is first converted to a byte object using `b'hello world!hello world!hello world!hello world!'`. This `byte` object is then passed to the `compress` function of the `zlib` library which returns a compressed version of the byte object.

The compressed version of the byte object is then printed, and finally, the compressed version of the byte object is passed to the `decompress` function of the `zlib` library which returns the original `byte` object. The decompressed `byte` object is then printed.

In this way, the code demonstrates the use of `zlib` library for data compression and decompression in Python.