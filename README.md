# bitoli <img src="https://github.com/retrotee/bitoli/blob/main/bitoli.jpeg" alt="bitoli" width="30"/>
**bitoli** is a Python package for adaptive compression and encryption of data. It provides simple methods to securely encode and decode data using AES encryption in CFB mode along with adaptive compression techniques.

## Features

- **Adaptive Compression:** Utilizes zlib for efficient data compression.
- **AES Encryption:** Implements AES encryption in CFB mode for secure data handling.
- **Base85 Encoding:** Supports encoding for non-compressed data.
- **Simple API:** Easy-to-use methods for encoding and decoding data.

## Installation

You can install bitoli using pip:

```bash
pip install bitoli
```

Usage
Here’s a simple example of how to use bitoli:

```python
from bitoli import encode, decode

key = "your_password"
data = "This is some data to encrypt and compress."

# Encode data
encoded_data = encode(data, key)
print("Encoded data:", encoded_data)

# Decode data
decoded_data = decode(encoded_data, key)
print("Decoded data:", decoded_data)
```

## API
```python
encode(data, key)
```
- Encrypts and compresses the data using the provided key.
<br>

```python
decode(data, key)
```
- Decompresses and decrypts the data using the provided key.

## License
This project is licensed under the MIT License.
