# Ciphers
Hardware implementation of light weight cryptographic ciphers PRESENT and ESF on logisim.

These ciphers can be run from command line by loading the 64-bit text and 80-bit key in the 3-bit address line RAM.

Steps to use:

1. Load the mem_img.txt file with your input data. It is the memory image that will be loaded in the RAM of the ciphers.
2. Run "java -jar logisim.jar PRESENT.circ -tty table -load mem_img.txt

Note:
The input format for the mem_img goes like this:
Row 0: Least Significant 32 bits of plain text.
Row 1: MSB 32 bits of plain text.
Row 2: LSB 32 bits of key.
Row 3: Next 32 bits of key.
Row 4: "xxxx" followd by Most significant 16 bits of the key.

All values have to be in Hex.


For additional details, contact: Piyush.ee317@ee.iitd.ac.in
