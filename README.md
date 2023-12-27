# Caesar Cipher 

## Encode-Decode
1. **Alphabet:** The script defines an alphabet list which includes lowercase letters twice to enable shifting without encountering an out-of-range error.
2. **`caesar` Function:** 
    - Takes in three parameters: `start_text` (the text to be encoded/decoded), `shift_amount` (the number of positions to shift), and `cipher_direction` (encode or decode).
    - Processes the text character by character:
        - Checks if the character is in the alphabet list.
        - If the character is a letter, it shifts its position in the alphabet by the specified `shift_amount` and constructs the encoded/decoded text.
        - If the character is not in the alphabet (e.g., space, number, or symbol), it keeps the character unchanged in the result.
    - Prints the encoded/decoded text.

3. **TODO-1:** Imports and prints a logo from an `art.py` file when the program starts.
4. **TODO-2:** Handles scenarios where the user enters a shift number greater than 26 by using modulus (%) to ensure the shift stays within the range of the alphabet.
5. **TODO-3:** Handles non-alphabetic characters like numbers, symbols, or spaces by retaining them in the encoded/decoded text without modification.
6. **TODO-4:** Implements a loop that allows the user to restart the program:
    - Asks the user if they want to continue by typing 'yes' or 'no' after each encryption/decryption cycle.
    - If the user types 'yes', it prompts for the direction (encode/decode), text, and shift amount again and calls the `caesar` function with the new inputs.
    - If the user types 'no', the program ends with a "Goodbye" message.

### Suggestions for Improvement:
- Error handling for non-integer inputs when asking for the shift amount.
- Option for the user to input uppercase letters and handle them appropriately.
- Incorporating more sophisticated ciphers or functionalities for encryption and decryption.
- Adding comments in the code for better readability and understanding.
