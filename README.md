# File compression using Huffman Coding

The main idea behind file compression is allocate less memory to more frequent characters and little bit more memory to less frequent characters which makes the memory attenuation possible.

### Steps

<!-- prettier-ignore -->
1. Compressing the file
     a. Store the frequency of all characters in a map.
     b. Sort the keys based on their frequency in non-decreasing order.
     c. Assign unique binary sequence to every key.
     d. Store these binary sequence in form of bits.
2. Decompressing the file
     a. Read the file in the same order as before.
     b. Replace the binary code into characters using the map.
