##  Random Password Generator 
A simple Python program to generate strong and secure random passwords using letters, numbers, and special characters.

## Features
* Generate passwords of any desired length
* Uses a mix of:
  * Uppercase letters (A–Z)
  * Lowercase letters (a–z)
  * Numbers (0–9)
  * Special characters (!, @, #, etc.)
* Simple and beginner-friendly code
* Fast and efficient

## Technologies Used
* Python 3
* Built-in Libraries:

  * `random`
  * `string`

## How It Works
1. The program asks the user to enter the desired password length.
2. It combines:
   * Letters (uppercase + lowercase)
   * Digits
   * Special characters
3. It randomly selects characters from this combined set.
4. These characters are joined together to form a secure password.
5. The generated password is displayed on the screen.

## Code
```
import random
import string

def generate_password(length):
    chars = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

length = int(input("Enter password length: "))
print("Generated Password:", generate_password(length))
```

## Output
```
Enter password length: 6
Generated Password: c!qjcK
```

## Author
Ayush Singh
GitHub: https://github.com/ayush893singh
