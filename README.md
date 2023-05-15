# LFSR_Password_Generator
This documentation provides an overview of the code for a password generator implemented using the tkinter library in Python. 
The password generator uses a linear feedback shift register (LFSR) algorithm to generate secure and random passwords.

The code begins by importing the necessary libraries:
The random library is used for generating random numbers and shuffling elements.
The tkinter library is used for creating the graphical user interface (GUI) for the password generator.
The messagebox module from tkinter is used to display warning and information messages.

The userInput() function is called when the "Use parameters" button is clicked. 
It retrieves the user input from the GUI and validates the entered values:
The function uses the global keyword to modify the global variables within the function.
It retrieves the minimum and maximum values for alphabets, numbers, and special characters from the GUI entries.
The password length is validated to ensure it falls within the specified range.
Random values are generated for alpha, num, and speciale based on the user input.

The generateSeed() function generates a seed for the LFSR algorithm:

The generateKey function generates a 16-bit key that is used to encrypt the password.

The passwordSeed function generates the password in plaintext.

The convertPassToBytes function converts the password to bytes.

The buildPass function applies XOR to the generated bits of the password using the key to encrypt the password.

The generatePassword function generates the password and converts the encrypted bytes back to a string.

The generate50 function generates 50 passwords and saves them to a file.

To use this script, run it in a Python environment with the tkinter module installed. 
When you run the script, a GUI window will appear. 
Enter the desired password parameters in the input fields and click the "Generate Password" button to generate a single password. 
Click the "Generate 50 Passwords" button to generate 50 passwords that will be saved in a file in the directory where the main code is saved.
