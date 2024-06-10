# CS240-MIPS-Image-Processing

This MIPS assembly program performs various image processing tasks, including image thresholding, matrix transformation, and cryptographic manipulation of image data. The program uses predefined matrices for transformations and processes images stored in the form of byte arrays.

Program Structure

The program is divided into three main parts:

1. Image Thresholding
2. Matrix Transformations
3. Image Cryptography

Image Processing Functions
1. Image Thresholding

The threshold function processes an image by applying a threshold value. Pixels above the threshold are set to 255, and those below are set to 0.

Input Parameters:
$a0: Input buffer address.
$a1: Output buffer address.
$a2: Image dimension (assuming a square image).
$a3: Threshold value.

2. Matrix Transformations

The transform function applies a transformation matrix to the image.

Input Parameters:
$a0: Input buffer address.
$a1: Output buffer address.
$a2: Transformation matrix address.
$a3: Image dimension (assuming a square image).

3. Image Cryptography

The cryptography function performs a cryptographic manipulation on the image data based on a simple modular arithmetic scheme.

Input Parameters:
$a0: Input buffer address.
$a1: Output buffer address.
$a2: Image dimension (assuming a square image).

Messages and Output

The program uses syscall instructions to print messages and array contents to the console, providing a clear output for each processing step.

File Handling

The program reads from and writes to image files, specified in the .data section. These files are in PGM (Portable GrayMap) format.

How to Run

Assemble the program using an assembler like SPIM or MARS.
Load the assembled program into the MIPS simulator.
Execute the program and observe the console output for test results and processed image data.
