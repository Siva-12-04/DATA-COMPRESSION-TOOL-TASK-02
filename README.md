# DATA-COMPRESSION-TOOL-TASK-04

NAME : Siva A

COMPANY : CODTECH IT SOLUTIONS

INTERN ID : CT08RJU

DOMAIN : C PROGRAMMING

DURATION : FEBRUARY 5th, 2025 to MARCH 5th, 2025 (4 WEEKS)

MENTOR : NEELA SANTHOSH

OVERVIEW OF THE PROGRAM:

The provided C program implements a Run-Length Encoding (RLE) compression and decompression tool, which is a straightforward method for reducing the size of data by encoding consecutive repeated characters. This program allows users to compress text files by replacing sequences of the same character with a count followed by the character, and to decompress files that have been previously compressed.

KEY FEATURES:

Run-Length Encoding (RLE):

RLE is a simple form of data compression that is particularly effective for data with many consecutive repeated characters. For example, the string "AAAABBBCCDAA" would be compressed to "4A3B2C1D2A", where each number represents the count of consecutive characters.

Functions:

compress(FILE *input_file, FILE *output_file):
This function reads characters from the input file and counts consecutive occurrences of each character. When a different character is encountered, it writes the count and the character to the output file.

decompress(FILE *input_file, FILE *output_file):
This function reads the compressed format from the input file, which consists of counts followed by characters, and reconstructs the original string by writing each character the specified number of times to the 

output file.

User Interaction:
The program features a command-line interface that prompts the user to choose between compressing or decompressing a file. The user is then asked to input the names of the input and output files.


File Handling:

The program uses standard file I/O functions to open, read, and write files. It includes error handling to manage issues such as failing to open files.

OUTPUT:

After Compression:

Input: AAAABBBCCDAA

Output (in compressed.txt): 4A3B2C1D2A

After Decompression:

Input: 4A3B2C1D2A

Output (in decompressed.txt): AAAABBBCCDAA

