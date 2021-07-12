# File compression using Huffman Coding

The main idea behind file compression is allocate less memory to more frequent characters and little bit more memory to less frequent characters which makes the memory attenuation possible.

### Steps

<!-- prettier-ignore -->
<ol>
<li>Compressing the file</li>
<ol type="a">
<li> Store the frequency of all characters in a map</li>
<li> Sort the keys based on their frequency in non-decreasing order</li>
<li> Assign unique binary sequence to every key</li>
<li> Store these binary sequence in form of bits </li>
</ol>
<li> Decompressing the file</li>
<ol type="a">
     <li> Read the file in the same order as before</li>
     <li> Replace the binary code into characters using the map</li>
</ol>
</ol>
