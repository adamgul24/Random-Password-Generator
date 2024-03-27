# Random Password Generator

## Overview
This Random Password Generator is a simple yet efficient Python script, perfect for generating strong, random passwords. It's designed to be user-friendly and is an essential tool for anyone's digital security toolkit.

## Features
### 1. Customizable Password Length
- Set the desired length for each password.

### 2. Batch Generation
- Generate multiple passwords at once.

### 3. Diverse Character Set
- Passwords are created using a mix of characters: uppercase, lowercase, numbers, and symbols.

### 4. Continuous Operation
- The script runs in a loop, allowing continuous password generation without restarting.

### 5. Simple User Interface
- Easy-to-follow prompts make the process straightforward.

## Usage
1. **Run the Script**
   - Execute in any Python environment.
2. **Enter Desired Length**
   - Input the length of your password when prompted.
3. **Specify Quantity**
   - Decide how many passwords you need.
4. **Receive Passwords**
   - The script outputs the generated passwords.

## Code Example
```python
import random

chars = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ123456!£$%^&*(`)"

while True:
    password_len = int(input("What length would you like your password to be: "))
    password_count = int(input("How many passwords would you like: "))
    for x in range(0, password_count):
        password = ""
        for x in range(0, password_len):
            password_char = random.choice(chars)
            password += password_char
        print("Here is your password: ", password)
