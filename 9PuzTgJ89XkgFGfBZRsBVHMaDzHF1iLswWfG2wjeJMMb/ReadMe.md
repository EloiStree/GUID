[<img width="222" height="222" alt="image" src="https://github.com/user-attachments/assets/7fddd701-4a70-4d61-bed8-49185c4ecf91" />](https://eloistree.github.io/GUID/9PuzTgJ89XkgFGfBZRsBVHMaDzHF1iLswWfG2wjeJMMb)   
https://eloistree.github.io/GUID/9PuzTgJ89XkgFGfBZRsBVHMaDzHF1iLswWfG2wjeJMMb   


# Demo,2D: Listen to NFC / Barcode

This tutorial demonstrates how to detect NFC tags and barcode scanner input.

Most NFC readers and barcode scanners behave like keyboards: they rapidly type an identifier followed by a terminating character, such as `\n` (Enter).

To detect a complete scan, listen for keyboard input and accumulate the characters. The input is considered complete when either:

* A configurable timeout expires between keystrokes.
* A terminating character such as `\n` is received.

Once either condition is met, the collected text can be validated and processed as the scanned NFC tag or barcode.

This version is more accurate (since it's the scanner that behaves like a keyboard, not the NFC tag itself) and reads more naturally for technical documentation.
