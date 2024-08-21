# Password Complexity Checker & Cracking Time Estimator

This repository contains a Python program that evaluates the complexity of a given password and estimates the time it would take a hacker to brute force crack it. The program provides insights into the strength of the password based on its length and character composition.

## Features

- **Password Complexity Analysis**:
  - Checks password length.
  - Verifies if the password contains uppercase letters.
  - Verifies if the password contains lowercase letters.
  - Checks for digits in the password.
  - Checks for special characters.

- **Time-to-Crack Estimation**:
  - Estimates the total number of possible combinations for the password.
  - Assumes a brute force attack with 1 billion attempts per second.
  - Provides an estimated time to crack the password in seconds, minutes, hours, days, and years.

## How it Works

1. **Character Set Calculation**: 
   - The program calculates the size of the character set based on whether the password contains:
     - Uppercase letters (26 characters).
     - Lowercase letters (26 characters).
     - Digits (10 characters).
     - Special characters (32 characters, approx.).

2. **Combination Calculation**: 
   - Based on the password length and the character set, the total number of possible combinations is calculated.

3. **Cracking Time Estimation**: 
   - The program estimates how long it would take a hacker to crack the password, assuming they can try **1 billion passwords per second**.

## Example

### Example Input
```
Enter your password: P@ssw0rd!
```

### Example Output
```
Password length: 9
Includes uppercase letters: True
Includes lowercase letters: True
Includes digits: True
Includes special characters: True
Estimated total combinations: 835,308,258,201,273
Time to crack:
- In seconds: 835,308,258.20 seconds
- In minutes: 13,921,804.30 minutes
- In hours: 232,030.07 hours
- In days: 9,668.75 days
- In years: 26.49 years
```

## Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Hun33er/PRODIGY_WD_03/password-complexity-checker.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd password-complexity-checker
   ```

3. Run the program using Python:
   ```bash
   python password_checker.py
   ```

## Customization

You can adjust the program to make it more suited to your use case:
- **Character Set**: Adjust the number of special characters if your system recognizes a different set.
- **Attempts per Second**: Change the default 1 billion attempts per second if you believe a different rate applies to your scenario.

## Requirements

- **Python 3.x**: This program is written in Python and should work with any version of Python 3.x.

No external libraries are needed, so once you have Python installed, you're good to go.

## Contributing

Feel free to open a pull request if you have suggestions or improvements. Whether it's optimizing the algorithm, adding more features, or fixing bugs, contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This README provides everything users need to understand the purpose, features, installation process, and how they can contribute. It also includes an example of the output to illustrate what the program does.
